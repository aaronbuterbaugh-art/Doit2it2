# Doit2it — Home Improvement App

A mobile-friendly AI home improvement app powered by Groq (free). Works on iPhone, Android, and desktop.

---

## Deploy to Vercel (free, ~10 minutes)

### Step 1 — Get your FREE Groq API Key
1. Go to https://console.groq.com
2. Sign up for a free account (no credit card needed)
3. Click "API Keys" → "Create API Key"
4. Copy the key (starts with `gsk_...`)

### Step 2 — Put the app on GitHub
1. Go to https://github.com and sign up (free)
2. Click the "+" icon → "New repository"
3. Name it `doit2it` → click "Create repository"
4. Click "uploading an existing file"
5. Unzip the downloaded folder and drag ALL files into GitHub
6. Click "Commit changes"

### Step 3 — Deploy on Vercel
1. Go to https://vercel.com and click "Sign up with GitHub"
2. Click "Add New Project"
3. Find and select your `doit2it` repo → click "Import"
4. Before clicking Deploy, click "Environment Variables" and add:
   - Name:  GROQ_API_KEY
   - Value: paste your key from Step 1
5. Click "Deploy" — takes about 1 minute

### Step 4 — Open on your phone
- Vercel gives you a free URL like `https://doit2it.vercel.app`
- Open it in Safari (iPhone) or Chrome (Android)
- Add to Home Screen for an app icon:
  - iPhone: tap the Share button → "Add to Home Screen"
  - Android: tap the 3-dot menu → "Add to Home Screen"

---

## Files in this project

```
doit2it/
├── public/
│   └── index.html      ← The entire app (HTML + CSS + JS)
├── api/
│   └── analyze.js      ← Serverless API (keeps your Groq key secret)
├── vercel.json         ← Routing config
├── package.json        ← Project config
└── README.md           ← This file
```

---

## How it works
- You describe your room in the app
- The app calls a secure Vercel server function
- The server calls Groq's free AI (Llama 3.3 70B model)
- The AI returns personalized design ideas, supply lists, and building plans
- Supply links open Home Depot, Lowe's, and Amazon searches
- Building plans are downloadable as text files
- Contractor section shows local professionals to hire

---

## Groq Free Tier Limits
- 30 requests per minute
- 14,400 requests per day
- No credit card required
- More than enough for personal use
