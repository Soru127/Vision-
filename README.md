# Vision-
# 👁️ Vision — AI Companion

Your intelligent friend, mentor, and digital companion powered by Groq AI.

---

## 🚀 GitHub + Vercel Deployment Guide

### Step 1 — GitHub Par Upload Karo

1. **GitHub.com** par jao aur login karo
2. **New Repository** banao — naam rakho `vision-chatbot`
3. **Public** select karo
4. **Create Repository** click karo

Phir apne computer mein terminal kholo aur yeh commands chalaao:

```bash
# Project folder mein jao
cd vision-project

# Git initialize karo
git init

# Saari files add karo
git add .

# First commit karo
git commit -m "Initial commit — Vision AI Chatbot"

# GitHub se connect karo (apna username daalo)
git remote add origin https://github.com/YOUR_USERNAME/vision-chatbot.git

# Push karo
git branch -M main
git push -u origin main
```

---

### Step 2 — Groq API Key Lao (Free!)

1. **console.groq.com** par jao
2. Sign up / Login karo
3. **API Keys** section mein jao
4. **Create API Key** click karo
5. Key copy karo — aise dikhegi: `gsk_xxxxxxxxxxxxxxxxxx`

---

### Step 3 — Vercel Par Deploy Karo

1. **vercel.com** par jao aur GitHub se login karo
2. **Add New Project** click karo
3. Apna `vision-chatbot` repository select karo
4. **Import** click karo
5. **Environment Variables** section mein:
   - Name: `GROQ_API_KEY`
   - Value: `gsk_xxxxxxxxxxxxxxxxxx` (apni key paste karo)
6. **Deploy** click karo
7. 2-3 minute wait karo ✅

---

### ✅ Done!

Aapko ek live URL milega jaise:
`https://vision-chatbot-username.vercel.app`

Yeh URL share kar sako mobile, desktop — kahi bhi kaam karega!

---

## 📁 Project Structure

```
vision-project/
├── pages/
│   ├── index.js          ← Frontend (UI)
│   └── api/
│       └── chat.js       ← Backend (Groq API)
├── package.json
├── next.config.js
├── .gitignore
├── .env.example
└── README.md
```

---

## 🔧 Local Development (Optional)

```bash
npm install
# .env.local file banao aur GROQ_API_KEY daalo
npm run dev
# Browser mein jao: http://localhost:3000
```
