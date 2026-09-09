<div align="center">
  <img src="https://raw.githubusercontent.com/8wcznkmy6b-del/AuraSnap-PB/main/AuraSnap.png?v=2" width="120" alt="AuraSnap Icon" />
  <h1>AuraSnap</h1>
  <p>A native, ultra-lightweight screenshot and system-level productivity toolkit for macOS.</p>
  <p>Screenshots, In-Place Translation, Radial Tiling, Mouse Enhancer, Cloud Image Hosting & Finder Context Menu.</p>
  <p>
    <a href="https://aurasnap.dpdns.org/"><img src="https://img.shields.io/badge/Official_Website-aurasnap.dpdns.org-0ea5e9?style=flat-square&logo=safari" alt="Website" /></a>
    <a href="https://github.com/8wcznkmy6b-del/AuraSnap-PB/releases"><img src="https://img.shields.io/badge/Latest_Release-v3.0.57-10b981?style=flat-square&logo=apple" alt="Release" /></a>
    <img src="https://img.shields.io/badge/macOS-14.0+-blue?style=flat-square" alt="macOS" />
    <img src="https://img.shields.io/badge/Architecture-Apple_Silicon_Native-purple?style=flat-square" alt="Apple Silicon" />
  </p>
  <p>
    <a href="README.md"><b>简体中文</b></a> | <a href="README_EN.md"><b>English</b></a>
  </p>
</div>

---

## 💡 Overview

**AuraSnap** is a native macOS productivity tool engineered from the ground up in pure Swift. Free from Electron bloat and excessive resource consumption, its idle background memory footprint stays below **40MB**.

Beyond pixel-accurate screenshot annotations, in-place AI translation, top-level floating pins, and seamless scrolling capture, AuraSnap integrates a **Liquid Glass Radial Window Manager**, **Mouse Hardware Profiles & Gesture Enhancer**, **Native Cloud Image Hosting (10+ Providers)**, and a **System-Level Finder Context Menu Extension**—delivering the power of multiple utility apps in one cohesive native experience.

---

## ✨ Key Features

### 🪟 Radial Window Manager
* **Apple Liquid Glass Material**: Supports refractive liquid glass styling across all dial shapes without stealing key input focus from active applications.
* **"Gravity Lens" Theme**: Seamless unibody disk design with a smooth glowing vector needle and a 1:1 real-time HUD layout indicator in the center.
* **Crystal Tints & Independent Highlight Glow**: 7 master crystal tints and 8 distinct highlight glow presets with customizable opacity, complemented by an interactive 1:1 cursor emulation testbed.
* **8-Direction Instant Snapping**: Hold middle click, side button, or modifier keys and flick the cursor to snap windows to halves, quadrants, center, or full screen; includes Stage Manager safety margins and smart complementary tiling.

### 🖱️ Mouse & Input Enhancer
* **Multi-Profile Mapping with Physical Device Awareness**: Manage independent button mapping profiles for office, gaming, or mobile mice. `DeviceMatcher` fingerprinting (Vendor ID, Product ID, Serial Number) automatically identifies hardware and switches profiles on the fly with live status capsules (🟢 Connected / 🟠 Disconnected / ⚪️ Unbound).
* **"Hold-and-Scroll" Multitasking Gestures**:
  * Hold a designated mouse side button (or middle button) and scroll the wheel to trigger custom workflows without affecting standard webpage scrolling;
  * Switch full-screen Spaces, cycle applications (`⌘Tab`), rotate through windows (`⌘\``), switch browser tabs, or zoom smoothly;
  * Integrated state machine guards against accidental clicks when releasing the button after scrolling.
* **Smooth Scrolling with App Whitelist**: Converts mechanical stepped scrolling into inertia-driven smooth scrolling; easily whitelist specific apps to maintain raw hardware input.
* **Linear Pointer & Independent Scroll Direction**: Decouples external mouse scroll direction from the trackpad, and eliminates macOS non-linear mouse acceleration for 1:1 tracking.

### ☁️ Native Image Hosting & Cloud Upload
* **10 Major Cloud Providers Supported**:
  * **S3 Ecosystem**: Amazon S3, Cloudflare R2, MinIO, Backblaze B2, DigitalOcean Spaces, Tencent Cloud COS (S3 compatible);
  * **Direct Cloud APIs**: Alibaba Cloud OSS, Qiniu KODO;
  * **Repositories & Geeks**: GitHub repository uploads, Custom Webhook / HTTP POST endpoints.
* **Format Conversion & Compression**: In-flight WebP, JPEG, and PNG encoding with adjustable quality sliders.
* **AI Smart Naming & Link Generation**: Automatically analyzes screenshot contents to suggest semantic filenames; copies Markdown, HTML, or plain URLs to the clipboard upon completion with native Toast HUD feedback.

### 📁 Finder Context Menu Extension (FinderSync)
* **Native Single-Tier Menu**: Runs in a sandboxed, decoupled `FinderSync` extension process adhering strictly to macOS design standards with zero clutter.
* **New File from Templates**: Instantly create files from right-click context (Word, Excel, PowerPoint, PDF, Markdown, Text, Shell, Python, Swift, `.env`, `.gitignore`) or custom project scaffolding.
* **Quick Copy / Move**: Prompts native system destination pickers directly, eliminating cumbersome nested menus.
* **Instant Path Copying**: Copy POSIX absolute paths, Shell-escaped paths, or file URLs directly to the clipboard.

### 🌐 In-Place AI Translation
* **In-Place Background Erasing & Re-Rendering**: Translates selected regions directly on the source image, preserving baseline typography, font weights, colors, and multi-column formatting.
* **Multiple Service Providers**: Includes a zero-setup Quick Translation channel alongside support for DeepL, Google Cloud, Azure, Baidu, Tencent, and Volcengine APIs.
* **Instant Pin Translation**: Right-click on any floating pin for instant re-translation and side-by-side comparison.

### 📌 Interactive Floating Pins
* **Top-Level Floating Overlays**: Pin screenshots, plain text, or clipboard images with 120Hz momentum zooming.
* **⌘-Drag to Export**: Hold `Command` and drag pinned windows directly into Slack, Teams, WeChat, Mail, or Finder folders.
* **Ghost Mode**: Enables mouse click-through to underlying documents while holding `Option` allows relocation.

### 📜 Scrolling Capture (Long Screenshots)
* **Dual-Engine Stitching**: Accelerated by Apple Accelerate (vDSP) to capture long web pages, terminal logs, and chat threads with continuous overlap stitching and fixed-element filtering.

### 🔍 Offline OCR (Text Recognition)
* **Native Apple Vision Acceleration**: Millisecond-level multi-language text extraction with smart table formatting, allowing one-click export into clean Markdown tables.

### 🎨 Background Beautifier Studio
* **Social Media Card Generation**: Extracts dominant colors into Morandi gradient backdrops or utilizes your 5K system wallpaper.
* **Two-Phase Pass-Through Pipeline**: Pixel-accurate window drop shadow synthesis ensuring zero annotation displacement when copying with shadows.

---

## ⌨️ Shortcuts Reference

| Feature | Default Shortcut | Action |
| :--- | :--- | :--- |
| **Capture Screen** | `⌥ + 1` (Option + 1) | Trigger capture with smart window snapping |
| **Restore Last Pin** | `⌥ + 2` (Option + 2) | Reopen the most recently closed pin |
| **Screenshot Gallery** | `⌥ + 3` (Option + 3) | Browse local capture history with offline search |
| **Instant OCR** | `⌥ + 4` (Option + 4) | Box-select and extract recognized text to Markdown |
| **Scrolling Capture** | `⌥ + 5` (Option + 5) | Enter scrolling capture mode |
| **Record GIF / Video** | `⌥ + 6` (Option + 6) | Record selected region to GIF / MP4 |
| **Background Beautifier** | `⌥ + 7` (Option + 7) | Open frame and background editor |
| **In-Place Translation** | `⌥ + T` (Option + T) | Translate selection or pin in-place |
| **Radial Window Manager** | Middle Click / Side Button / `Fn` / `⌥` Drag | Summon 8-direction Liquid Glass radial wheel |
| **Half-Screen Snap** | `⌃ + ⌥ + ←` / `→` / `↑` / `↓` | Snap active window to Left / Right / Top / Bottom half |
| **Maximize / Center** | `⌃ + ⌥ + ↩` / `C` | Maximize window / Center on screen |
| **Corner Quadrants** | `⌃ + ⌥ + U` / `I` / `J` / `K` | Snap to Top-Left / Top-Right / Bottom-Left / Bottom-Right |
| **Clipboard to Pin** | `⌘ + ⌥ + T` | Create pinned window from clipboard content |
| **Pin Click-Through** | `⌥ + G` (Option + G) | Toggle click-through mode (Hold `⌥` to move) |
| **Quick Cloud Upload** | `⌥ + U` (Option + U) | Upload selected capture to default cloud storage |

> 💡 **Independent Global Hotkeys**: Every global shortcut features an independent toggle under **Preferences** ➔ **Shortcuts**. Disabled shortcuts release their keybindings completely, preventing conflicts with Final Cut Pro, Xcode, or Photoshop.

---

## 📥 Download & Installation

1. Go to the GitHub [**Releases**](https://github.com/8wcznkmy6b-del/AuraSnap-PB/releases) page.
2. Download the latest `AuraSnap.dmg` or `AuraSnap.app.zip` (**`v3.0.57`**).
3. Drag `AuraSnap.app` into your **Applications** folder.
4. On first launch, follow the prompts to grant **Screen Recording** and **Accessibility** permissions.

---

## 🛡 Privacy & Local-First

AuraSnap adheres to a strict **Local-First** architecture:
* Screen captures, OCR, scrolling stitching, window management, mouse remapping, and Finder actions run **100% locally on your Mac**;
* Image data is never uploaded unless you explicitly request cloud uploads or online translation services.

---

## 💎 License & Pro Edition

AuraSnap offers generous free daily quotas for core features.

Upgrade to **Pro Edition** to unlock unlimited high-speed translation, lossless long screenshot exports, HD recording, cloud image hosting, and premium themes:

* 🛒 **Official Store**: [Creem Store (https://www.creem.io/stores/aurasnap)](https://www.creem.io/stores/aurasnap)
* 💳 **Pricing**: Annual Subscription (~$0.83/mo) or Lifetime License ($19.9 Lifetime).
* 🔑 **Activation**: Enter your license key under **Preferences** ➔ **About** for immediate activation.

---

<div align="center">
  <sub>AuraSnap - Native All-in-One Productivity & Screenshot Toolkit for macOS.</sub><br>
  <sub>🌐 Official Website: <a href="https://aurasnap.dpdns.org/">https://aurasnap.dpdns.org/</a></sub>
</div>
