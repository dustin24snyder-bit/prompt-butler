# Prompt Butler 🦝

*"Allow me to refine that, sir."*

A skill-aware prompt generator that turns a rough idea into an exhaustively detailed,
portable prompt for ChatGPT, Claude, and Gemini. Single static page — no build step.

**Live site:** `https://<your-username>.github.io/<repo-name>/`

## Features
- Detailed / Concise / Template / Agent prompt formats
- Prioritized "improve" questions (Critical / High / Mid)
- Image & GIF/video prompt mode (Midjourney, DALL·E, Stable Diffusion, Sora)
- **Rocco's services** on every polished prompt:
  - 🎨 Create the image — free in-browser generation via Pollinations.ai (Bing Image Creator fallback)
  - 🌐 Translate — 11 languages via the free MyMemory API (Google Translate fallback); non-English input is detected and offered an instant translate-&-polish
  - 🪄 Humanize — instant local tone rewrites (warm / punchier / professional)
  - 💬 Get coaching — opens your own AI with a prompt-coach meta-prompt
- One-click open in ChatGPT / Claude / Gemini (remembers your favorite)
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
