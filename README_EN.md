<div align="center">
  <img src="https://raw.githubusercontent.com/8wcznkmy6b-del/AuraSnap-PB/main/AuraSnap.png?v=2" width="120" alt="AuraSnap Icon" />
  <h1>AuraSnap</h1>
  <p>A native screenshot and productivity toolkit for macOS.</p>
  <p>Screenshots & annotation, in-place translation, scrolling capture, screen recording, clipboard history, window tiling, mouse enhancements and Finder actions — in one native app.</p>
  <p>
    <a href="https://aurasnapapp.com/"><img src="https://img.shields.io/badge/Website-aurasnapapp.com-0ea5e9?style=flat-square&logo=safari" alt="Website" /></a>
    <a href="https://github.com/8wcznkmy6b-del/AuraSnap-PB/releases/latest"><img src="https://img.shields.io/github/v/release/8wcznkmy6b-del/AuraSnap-PB?style=flat-square&logo=apple&label=Latest&color=10b981" alt="Release" /></a>
    <img src="https://img.shields.io/badge/macOS-14.0+-blue?style=flat-square" alt="macOS" />
    <img src="https://img.shields.io/badge/Apple_Silicon-Native-purple?style=flat-square" alt="Apple Silicon" />
  </p>
  <p>
    <a href="README.md"><b>简体中文</b></a> | <a href="README_EN.md"><b>English</b></a>
  </p>
</div>

---

## 📥 Installation

### Option 1: Homebrew (recommended)

```bash
brew install --cask 8wcznkmy6b-del/tap/aurasnap
```

- Opens right away after install; macOS won't block it.
- Update from inside the app afterwards; `brew upgrade --cask aurasnap` also follows new releases.
- Uninstall: `brew uninstall --cask aurasnap`. To also remove settings and clipboard history: `brew uninstall --zap --cask aurasnap`.

### Option 2: Download the DMG

1. Download the latest `AuraSnap-<version>.dmg` from [**Releases**](https://github.com/8wcznkmy6b-del/AuraSnap-PB/releases/latest);
2. Open it and drag `AuraSnap.app` into **Applications**;
3. If macOS says the developer can't be verified on first launch, click **Open Anyway** at the bottom of **System Settings › Privacy & Security**, or run:
   ```bash
   xattr -dr com.apple.quarantine /Applications/AuraSnap.app
   ```

### First launch

Follow the welcome guide to grant **Screen Recording** and **Accessibility**. Microphone, camera and other permissions are requested only when you first use them.

---

## 💡 Overview

**AuraSnap** is written natively in Swift — no Electron. It lives in the menu bar and stays light.

Screenshots, annotation, text recognition, in-place translation, scrolling capture, screen recording, clipboard history, window tiling, mouse enhancements and Finder actions: one lightweight native app instead of several always-running utilities.

---

## ✨ Features

### 📸 Screenshots & Annotation
* **Capture**: region capture, smart window detection with edge snapping, capture straight to clipboard, delayed capture; optionally hide desktop icons while capturing.
* **Annotation tools**: rectangle (rounded, rotatable), arrow (including curved), line, pen / highlighter, text, callout, numbered steps, stickers, spotlight, magnifier, watermark; solid, dashed and dash-dot line styles.
* **Privacy**: several mosaic styles, one-click auto-redact of sensitive info, and smart erase that removes text or objects and fills in the background.
* **More**: subject cutout, color picker, pixel ruler; click any annotation to adjust it again; customizable toolbar order and groups.
* **After capture**: keep screenshots as **sticky notes** on the screen edge or on a **clothesline** across the top of the screen. Click to copy, double-click to pin, long-press to edit, drag into an app to send or into a folder to save.
* **Edit existing images**: right-click an image in Finder and choose **Edit Image**, or open it with AuraSnap, to use the same editor.

### 🌐 In-Place Screenshot Translation
* **Keeps the layout**: select foreign text and the translation is drawn back in place, matching the original color, size, weight and layout.
* **System translation (default)**: on macOS 15+, uses Apple's offline translation — no setup, nothing leaves your Mac.
* **Your own API keys**: Baidu, Microsoft, DeepL, Google, Tencent, Volcengine, Youdao image translation and more, with automatic fallback to other configured services.
* **Pin translation**: translate pinned images too, and copy translated text by selecting it.
* **Mouse selection translation**: hold a side button while selecting text to see the translation next to the cursor.

### 🤖 AI Assistant
* Type an instruction after capturing, or tap **Explain / Translate / Extract**; works with system capabilities or your own API key.
* Conversations are saved and can be continued in a separate history window.

### 📌 Floating Pins
* Pin screenshots, text or clipboard images on top of everything; zoom with the scroll wheel or pinch.
* Hold `⌘` and drag a pin straight into chat apps, Mail or Finder.
* **Click-through mode**: interact with what's underneath; hold `⌥` to move the pin.
* Edit, recognize text and translate right on the pin.

### 📜 Scrolling Capture
* Stitches web pages, code, chats and terminal logs in real time with a live preview; removes sticky headers, fixed footers and static sidebars.
* Vertical and horizontal scrolling, with an adjustable area before you start.

### 🎬 Screen Recording
* Record a region to MP4 / GIF at native resolution and 60 fps, with system audio, microphone, and on-screen clicks and keystrokes.
* Camera overlay and simple trimming after recording.
* **Auto zoom**: zooms in on clicks and typing and follows smoothly, Screen Studio style.

### 🔍 Text Recognition (OCR)
* Offline multi-language text and QR code recognition with Apple Vision; keeps paragraphs, copies tables as Markdown.
* `⌥4`, select, and the result appears; `⌘↩` copies, closes, and returns the keyboard to your previous window.

### 📋 Clipboard History
* Records text, images, files, links and colors; type to search, filter by category or source app.
* Card popup or a shelf along the bottom / top of the screen; hover to preview, recognize text in images on demand.
* Multi-select to paste items one by one or merged; **Paste as…** plain text, upper / lower case, formatted JSON, URL or Base64 encode / decode.
* **Favorites** for snippets, images and files, plus custom tags.
* Ignore specific apps (e.g. password managers) and skip password content automatically; works with iPhone Universal Clipboard.

### 🪟 Window Tiling
* Keyboard tiling: halves, quarters, thirds (1/3, 2/3), maximize, center, move to another display, restore.
* **Radial gesture wheel**: hold the wheel button, a side button or a modifier and nudge the mouse to snap in 8 directions; Liquid Glass wheel with several themes.
* Complementary tiling (fills the other side), window gaps, cross-display moves.

### 🖱️ Mouse Enhancements
* **Smooth scrolling**: trackpad-like scrolling for regular wheels, with per-app exceptions; reverse the external mouse wheel independently.
* **Pointer acceleration**: system default, linear, or a custom curve.
* **Button mapping**: map side-button clicks, hold-and-scroll and drag gestures to switching Spaces, apps / windows / tabs, zoom, or any shortcut; wheel tilt left / right; per-app mappings with conflict warnings against system shortcuts.
* **Multiple mouse profiles**: switch automatically per device; wired / 2.4G / Bluetooth of the same mouse count as one.
* **Mouse hardware settings**: for Razer and MCHOSE mice, set DPI stages, polling rate and lighting (including per-LED colors) saved to onboard memory, and see battery level; steps aside when the official driver is installed.

### ☁️ Image Hosting Upload
* Amazon S3, Cloudflare R2, MinIO, Backblaze B2, DigitalOcean Spaces, Tencent COS, Aliyun OSS, Qiniu KODO, GitHub repositories and custom webhooks.
* Copies the link automatically (Markdown / HTML / plain URL); WebP / JPEG / PNG with adjustable quality.

### 📁 Finder Context Menu
* Create new files in empty space: Office documents, Markdown, text and code templates, plus your own templates.
* Copy path, open in Terminal / editor, compress / extract, image tools (convert, resize, recognize text), copy / move to favorite folders.
* `⌘X` to cut and `⌘V` to move files in Finder; custom script actions.

---

## ⌨️ Default Shortcuts

| Action | Default |
| :--- | :--- |
| Capture | `⌥1` |
| Capture to clipboard | `⌥⇧1` |
| Delayed capture | `⌃⌥1` |
| Restore last pin | `⌥2` |
| Clipboard history | `⌥3` |
| Text recognition (OCR / QR) | `⌥4` |
| Scrolling capture | `⌥5` |
| Screen recording | `⌥6` |
| Screenshot beautifier | `⌥7` |
| Screenshot translation | `⌥8` |
| Clipboard to pin | `⌘⌥T` |
| Upload clipboard image | `⌘⌥U` |
| Toggle pin click-through | `⌥G` |
| Left / right / top / bottom half | `⌃⌥←` `→` `↑` `↓` |
| Maximize / center / restore | `⌃⌥↩` / `⌃⌥C` / `⌃⌥⌫` |
| Quarters | `⌃⌥U` `I` `J` `K` |
| Radial tiling wheel | Hold wheel button / side button / modifier and nudge the mouse |

While capturing, single keys pick tools (e.g. `R` rectangle, `A` arrow, `T` text, `M` mosaic, `X` pixel ruler). See all of them in **Settings › Shortcuts**.

> 💡 Every global shortcut can be changed or turned off individually; turned-off shortcuts are fully released for other apps. Single keys and F1–F12 are supported too.

---

## 🛡 Privacy: Local First

* Capture, annotation, OCR, scrolling capture, recording, clipboard, tiling, mouse and Finder features all run locally on your Mac;
* Content is sent only when you choose online translation, the AI assistant (with your own key) or an image host — and only to the provider you picked;
* Clipboard history stays on your Mac and skips password managers and other sensitive content.

---

## 💎 Free & Pro

Most features are free. **Clipboard history, the AI assistant and screenshot translation are completely free.**

**Pro** unlocks unlimited text recognition, unlimited scrolling capture length, advanced tiling and Finder actions, mouse button mapping and more.

* 🛒 **Buy**: [aurasnapapp.com/pricing](https://aurasnapapp.com/pricing)
* 💳 **Pricing**: $1.49 / month, $3.99 / quarter, $9.99 / year (about $0.83 / month), or $19.99 one-time
* 🔑 **Activate**: enter your license key in **Settings › About**

---

## 💬 Feedback

Found a bug or want a feature? Open an [Issue](https://github.com/8wcznkmy6b-del/AuraSnap-PB/issues).

---

<div align="center">
  <sub>AuraSnap - Native All-in-One Productivity & Screenshot Toolkit for macOS.</sub><br>
  <sub>🌐 Website: <a href="https://aurasnapapp.com/">https://aurasnapapp.com/</a></sub>
</div>
