# 🚀 Chore Quest - Hackathon Prototype

Welcome to Chore Quest! This is a gamified household chore management app designed to make chores visible, fair, and rewarding.

## 🛠️ Tech Stack
- **Frontend:** Next.js 15 (App Router), TypeScript, Tailwind CSS
- **Backend/Auth:** Supabase (PostgreSQL + Supabase Auth)
- **Hosting:** Vercel (Recommended)
- **Icons:** Lucide React

## 🚀 Quick Start Guide (Local Setup)

### 1. Install Dependencies
Open your terminal in the project folder and run:
```bash
npm install
```

### 2. Environment Variables
Create a file named `.env.local` in the root directory and add your Supabase credentials:
```env
NEXT_PUBLIC_SUPABASE_URL=your_supabase_project_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key
```

### 3. Database Setup
1. Log into your [Supabase Dashboard](https://app.supabase.com/).
2. Go to the **SQL Editor** tab.
3. Copy the contents of `supabase/schema.sql` and paste it into the editor.
4. Click **Run**.

### 4. Run the App
```bash
npm run dev
```
Open [http://localhost:3000](http://localhost:3000) in your browser.

---

## ☁️ Deployment (Live URL)

1. **Push to GitHub:** Create a repo and push this code.
2. **Connect to Vercel:** Import the repo at [vercel.com](https://vercel.com).
3. **Add Env Vars:** In Vercel project settings, add the `NEXT_PUBLIC_SUPABASE_URL` and `NEXT_PUBLIC_SUPABASE_ANON_KEY`.
4. **Deploy:** Click deploy and share your link!

## 🎮 Core Loop for Demo
1. **Sign Up:** Create a new account.
2. **Create Chore:** (As Organizer) Add a chore with a point value and assign it to a member.
3. **Complete Chore:** (As Member) Mark a chore as complete.
4. **Award Points:** If "Approval Required" was off, points are added immediately. If on, the Organizer must approve it in the **Review** tab.
5. **Recognition:** Check the **Family** tab to see the point leaderboard.
