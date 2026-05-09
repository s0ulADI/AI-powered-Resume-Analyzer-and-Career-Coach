# 🧠 ResumeIQ — AI-Powered Resume Analyzer & Career Coach

> An intelligent resume analysis tool built with the Claude AI API. Get ATS compatibility scores, keyword gap analysis, strengths/weaknesses breakdown, and an AI-rewritten professional summary — instantly.

![ResumeIQ Screenshot](https://img.shields.io/badge/Powered%20By-Claude%20AI-6affb4?style=for-the-badge&labelColor=0a0a0f)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Live-brightgreen?style=for-the-badge)

---

## ✨ Features

- **ATS Score (0–100)** — Measures how well your resume matches a job description using the same logic as Applicant Tracking Systems
- **Keyword Gap Analysis** — Instantly see which keywords from the JD are present or missing in your resume
- **Strengths & Weaknesses** — Honest, specific feedback on what's working and what's hurting your chances
- **Top Improvement Actions** — Prioritized, actionable suggestions to boost your score
- **AI-Rewritten Summary** — Claude rewrites your professional summary tailored to the specific job

---

## 🚀 Getting Started

### 1. Clone the repo
```bash
git clone https://github.com/yourusername/resumeiq.git
cd resumeiq
```

### 2. Open in browser
This is a pure frontend app — no server needed.
```bash
open index.html
# or just drag index.html into your browser
```

### 3. Get your Claude API key
- Sign up at [console.anthropic.com](https://console.anthropic.com)
- Create an API key (free tier available)
- Paste it into the API Key field in the app

> **Privacy**: Your API key is never sent to any server other than Anthropic's API directly. It stays in your browser session only.

---

## 🛠 Tech Stack

| Layer | Tech |
|---|---|
| Frontend | Vanilla HTML, CSS, JavaScript |
| AI | [Anthropic Claude API](https://docs.anthropic.com) (`claude-sonnet-4`) |
| Fonts | Syne, DM Mono, Instrument Serif (Google Fonts) |
| Deployment | Any static host (GitHub Pages, Vercel, Netlify) |

No build step. No dependencies. No backend. Just open and use.

---

## 📁 Project Structure

```
resumeiq/
├── index.html        # Entire app (self-contained)
└── README.md         # This file
```

---

## 🧩 How It Works

1. User pastes their **resume text** and a **job description**
2. The app constructs a structured prompt and calls the **Claude API** directly from the browser
3. Claude returns a JSON object containing the score, keywords, feedback, and rewritten summary
4. The app renders the results in a clean, interactive UI

### Prompt Engineering
The app uses a structured prompt that instructs Claude to return a specific JSON schema, making parsing reliable and the UI consistent. The model used is `claude-sonnet-4-20250514` for the best balance of quality and speed.

---

## 🚢 Deployment

### GitHub Pages
1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Set source to `main` branch, `/ (root)`
4. Visit `https://yourusername.github.io/resumeiq`

### Vercel / Netlify
Just drag the folder into Vercel or Netlify's dashboard — zero config needed.

---

## 🤝 Contributing

Pull requests welcome! Ideas for future features:
- [ ] PDF resume upload support
- [ ] Multi-job comparison mode
- [ ] LinkedIn profile URL import
- [ ] Export results as PDF report
- [ ] Cover letter generator

---

## 📝 License

MIT — free to use, modify, and distribute.

---

## 🙏 Acknowledgements

Built with [Anthropic's Claude API](https://www.anthropic.com). This project was created for the **Vibe Coding Hackathon** to demonstrate real-world AI application development with modern web technologies.

---

<p align="center">Made with ✦ and Claude AI</p>
