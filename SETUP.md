# NHAPP Setup Guide (WhatsApp Style Clone)

## 1. Supabase Setup
1.  **Create a New Project** on [Supabase](https://supabase.com).
2.  **Run SQL**: Go to the SQL Editor and paste the contents of `supabase_schema.sql`.
3.  **Enable Storage**: Create a bucket called `avatars` and set it to public.
4.  **Get API Keys**: 
    - Go to Project Settings -> API.
    - Copy your `Project URL` and `anon public` key.

## 2. Firebase Cloud Messaging (FCM) Setup
1.  **Create a New Project** on [Firebase Console](https://console.firebase.google.com).
2.  **Add Android App**: Use package name `com.nhapp`.
3.  **Download `google-services.json`**: Place it in the `app/` directory of your Android project.

## 3. Push Notifications Strategy
- Use **Supabase Edge Functions** to trigger FCM when a recipient is offline.

## 4. Android App Configuration
1.  Open `AndroidManifest.xml` and add:
    ```xml
    <uses-permission android:name="android.permission.INTERNET" />
    <uses-permission android:name="android.permission.POST_NOTIFICATIONS" />
    ```
2.  The package name is `com.nhapp`.

## 5. Running the App
1.  Sync Gradle.
2.  Run the app.
