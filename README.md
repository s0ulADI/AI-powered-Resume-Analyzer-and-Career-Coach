# 🧠 ResumeIQ — AI-Powered Resume Analyzer & Career Coach

> An intelligent resume analysis tool built with the Google Gemini AI API. Get ATS compatibility scores, keyword gap analysis, strengths/weaknesses breakdown, and an AI-rewritten professional summary — instantly and for free.

![ResumeIQ](https://img.shields.io/badge/Powered%20By-Google%20Gemini%20AI-6affb4?style=for-the-badge&labelColor=0a0a0f)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)
![No Backend](https://img.shields.io/badge/Backend-None%20Required-brightgreen?style=for-the-badge)
![Free](https://img.shields.io/badge/API-100%25%20Free-orange?style=for-the-badge)

---

## ✨ Features

- **ATS Score (0–100)** — Measures how well your resume matches a job description using the same logic as Applicant Tracking Systems
- **Keyword Gap Analysis** — Instantly see which keywords from the JD are present or missing in your resume
- **Strengths & Weaknesses** — Honest, specific feedback on what's working and what's hurting your chances
- **Top Improvement Actions** — Prioritized, actionable suggestions to boost your score
- **AI-Rewritten Summary** — Gemini rewrites your professional summary tailored to the specific job

---

## 🚀 Getting Started

### 1. Clone the repo
```bash
git clone https://github.com/yourusername/resumeiq.git
cd resumeiq
```

### 2. Open in browser
This is a pure frontend app — no server, no install needed.
```bash
open index.html
# or just drag index.html into your browser
```

### 3. Get your FREE Gemini API key
- Go to [aistudio.google.com/app/apikey](https://aistudio.google.com/app/apikey)
- Sign in with your **Google account**
- Click **"Create API Key"** → **"Create API key in new project"**
- Copy the key (it looks like `AIzaSy...`)

### 4. Use the app
- Paste your API key into the **"Gemini API Key"** field in the app
- Paste your resume text
- Paste the job description you're targeting
- Click **"Analyze My Resume"**

> **No code editing required.** The API key field is built into the UI.

> **Privacy**: Your API key is sent only to Google's Gemini API directly from your browser. It is never stored or sent anywhere else.

---

## 🛠 Tech Stack

| Layer | Tech |
|---|---|
| Frontend | Vanilla HTML, CSS, JavaScript |
| AI | [Google Gemini API](https://aistudio.google.com) (`gemini-1.5-flash`) |
| Fonts | Syne, DM Mono, Instrument Serif (Google Fonts) |
| Deployment | Any static host (GitHub Pages, Vercel, Netlify) |

No build step. No npm. No backend. Just open and use.

---

## 📁 Project Structure

```
resumeiq/
├── index.html        # Entire app (self-contained, single file)
├── README.md         # This file
├── LICENSE           # MIT License
└── .gitignore        # Ignores OS junk and .env files
```

---

## 🧩 How It Works

1. User pastes their **resume text** and a **job description**
2. The app builds a structured prompt and calls the **Gemini API** directly from the browser
3. Gemini returns a JSON object with the score, keywords, feedback, and rewritten summary
4. The app renders everything in a clean, interactive dark UI

### Prompt Engineering
The app uses a structured prompt instructing Gemini to return a strict JSON schema, making parsing reliable and results consistent. Model used: `gemini-1.5-flash` for best speed and quality on the free tier.

---

## 🚢 Deployment

### GitHub Pages (free hosting)
1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Set source to `main` branch, `/ (root)`
4. Your live URL: `https://yourusername.github.io/resumeiq`

### Vercel or Netlify
Drag the folder into [vercel.com](https://vercel.com) or [netlify.com](https://netlify.com) — zero config, instant deploy.

---

## 🤝 Contributing

Pull requests welcome! Ideas for future features:
- [ ] PDF resume upload & text extraction
- [ ] Multi-job comparison mode
- [ ] LinkedIn profile URL import
- [ ] Export results as PDF report
- [ ] Cover letter generator

---

## 📝 License

MIT — free to use, modify, and distribute.

---

