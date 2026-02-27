# NHAPP Web Companion Setup Guide

This is a Next.js 14 web application designed to accompany the NHAPP Android app. It uses the same Supabase backend.

## 1. Prerequisites
- Node.js installed.
- Supabase project established (same as Android app).

## 2. Configuration
1.  Navigate to `C:\Users\Y Venkat\.gemini\antigravity\scratch\nhapp-web`.
2.  Rename `.env.local.example` to `.env.local`.
3.  Add your Supabase URL and Anon Key.

## 3. Running Locally
```bash
npm install
npm run dev
```
Visit `http://localhost:3000` in your browser.

## 4. Deployment to Vercel
1.  Push this code to a GitHub repository.
2.  Import the repository into Vercel.
3.  Add the environment variables in the Vercel dashboard.
4.  Vercel will automatically deploy the app.

## Features Included:
- **Premium Design**: Dark mode, glassmorphic effects, and fluid animations using Framer Motion.
- **Auth Flow**: Magic Link authentication placeholder (ready for Supabase Auth).
- **Chat Interface**: Fully responsive, WhatsApp-style layout with side-scrolling chats and message bubbles.
- **Responsive**: Works on desktop and mobile browsers.
