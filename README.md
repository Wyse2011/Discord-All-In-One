# Discord Markdown Editor

A web-based markdown editor for composing Discord messages with live preview and copy-paste output segments.

## Features
- Full Discord markdown formatting toolbar (Bold, Italic, Underline, Strikethrough, Spoiler, Headers, Lists, Blockquotes, Code, Links)
- Live Discord-style preview panel
- Automatic text segmentation for Standard (2000 chars) and Discord Nitro (4000 chars) limits
- Word-boundary-aware splitting so words are never cut mid-segment
- One-click copy per segment

## How to Run in IntelliJ IDEA

### Option 1: Built-in Browser Preview (Recommended)
1. Open IntelliJ IDEA
2. Go to **File → Open** and select this project folder
3. Open `index.html` in the editor
4. Click the browser icon (Chrome/Firefox/Edge) that appears in the top-right corner of the editor
5. The app will open in your default browser

### Option 2: Run with a Local Server (via IntelliJ's built-in server)
1. Open `index.html`
2. Right-click in the editor → **Open In → Browser**

### Option 3: Static File Server via Terminal
From the project root, run one of the following:
```bash
# Python 3
python -m http.server 8080

# Node.js (if installed)
npx serve .
```
Then open `http://localhost:8080` in your browser.

## Project Structure
```
discord-editor/
├── index.html      # Main application (self-contained, no dependencies)
└── README.md       # This file
```

## Notes
- No build step required — the app is a single self-contained HTML file
- All CSS and JavaScript are embedded inline
- Google Fonts are loaded from CDN (requires internet connection for full typography)
- Works in any modern browser (Chrome, Firefox, Edge, Safari)
