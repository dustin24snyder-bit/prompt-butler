# Prompt Butler 🦝

*"Allow me to refine that, sir."*

A skill-aware prompt generator that turns a rough idea into an exhaustively detailed,
portable prompt for ChatGPT, Claude, and Gemini. Single static page — no build step.

**Live site:** `https://<your-username>.github.io/<repo-name>/`

## Features
- Detailed / Concise / Template / Agent prompt formats
- Prioritized "improve" questions (Critical / High / Mid)
- Image & GIF/video prompt mode (Midjourney, DALL·E, Stable Diffusion, Sora)
- Attach files & images for extra context
- Local version history + saved-prompt library (stored in your browser)
- Mobile-friendly + "Add to Home Screen" (PWA manifest + icons)
- **⚡ Turbo:** optional, uses *your own* Anthropic API key (entered at runtime,
  stored only in your browser's `localStorage`, sent directly to Anthropic)

## 🔒 Security
This repo contains **no API keys**. The Turbo key is entered by each user in their own
browser and never leaves their device except as a direct call to Anthropic. **Never commit
an API key to this repo.**

## Run locally
Just open `index.html` in a browser, or serve it:

```bash
python -m http.server 8000   # then visit http://localhost:8000
```

## Deploy (GitHub Pages)
Push to GitHub → Settings → Pages → Source: `main` branch, `/ (root)` → Save.
