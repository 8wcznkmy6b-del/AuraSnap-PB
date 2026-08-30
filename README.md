<div align="center">
  <img src="https://raw.githubusercontent.com/8wcznkmy6b-del/AuraSnap-PB/main/AuraSnap.png" width="120" alt="AuraSnap Icon" />
  <h1>AuraSnap</h1>
  <p>专为 macOS 打造的原生截图工具箱</p>
  <p>集截图、原地翻译、屏幕贴图、长截图、文字识别 (OCR)、内容擦除与背景美化于一体。</p>
  <p>
    <a href="https://aurasnap.dpdns.org/"><img src="https://img.shields.io/badge/官网-aurasnap.dpdns.org-0ea5e9?style=flat-square&logo=safari" alt="Website" /></a>
    <a href="https://github.com/8wcznkmy6b-del/AuraSnap-PB/releases"><img src="https://img.shields.io/badge/最新版本-v3.0.16-10b981?style=flat-square&logo=apple" alt="Release" /></a>
    <img src="https://img.shields.io/badge/macOS-14.0+-blue?style=flat-square" alt="macOS" />
    <img src="https://img.shields.io/badge/架构-Apple_Silicon_原生-purple?style=flat-square" alt="Apple Silicon" />
  </p>
  <p>
    <a href="README.md"><b>简体中文</b></a> | <a href="README_EN.md"><b>English</b></a>
  </p>
</div>

---

## 💡 产品简介

AuraSnap 是一款纯 Swift 原生开发的 Mac 截图效率工具。没有 Electron 的臃肿和高内存占用，日常驻留内存通常小于 40MB。

不仅满足日常截图标注与贴图需求，更专注于解决看外文文档、长代码长网页截屏、社媒分享图美化等实际场景中的繁琐步骤。

---

## ✨ 核心功能

### 🌐 翻译
* **原地排版渲染 (In-Place Rendering)**：框选外文区域，直接在原图对应位置擦除背景并重新绘制译文；自动提取并继承源图的基线高度、字重字阶与文本色彩，保留原始段落与列表版式，告别繁琐的复制粘贴。
* **多服务商与快捷模式**：内置免配置的快捷翻译通道；同时支持接入 DeepL、Google Cloud Translation、Microsoft Azure、百度、腾讯、火山引擎等标准 API 服务。
* **贴图即时对照**：置顶悬浮的贴图支持右键即时翻译、强制重新翻译与原文对照，满足多任务阅读需求。

### 📌 屏幕贴图与快捷交互
* **置顶悬浮与平滑缩放**：一键将截图、纯文本或剪贴板图片固定在屏幕最上层，触控板或滚轮双指无级缩放。
* **⌘ 键直接拖拽外发**：按住 `Command` 键拖拽贴图，可直接丢进微信、飞书、钉钉、邮件发送，或拖入访达保存为图片。
* **点击穿透 (Ghost Mode)**：开启穿透后，鼠标可直接点击贴图下方的代码或网页；长按 `Option` 可临时选中移动。

### 📜 平滑长截图
* **自由滚动拼接**：支持聊天记录、长网页、终端日志的长截图捕获，平滑滚动即时拼接，带右侧实时预览地图。

### 🔍 离线文字识别 (OCR)
* **系统原生引擎加速**：多语言混合秒级识别，支持直接框选提取、截图后提取或从外部拖入图片提取。
* **智能排版还原**：自动识别段落与表格结构，支持一键复制为 Markdown 格式表格，智能去除多余换行与空格。

### 🎨 截图背景美化
* **一键生成社媒卡片**：自动提取截图主色调生成莫兰迪渐变背景，或直接使用系统 5K 桌面壁纸作为衬底。
* **拟真光影效果**：提供 macOS 原生窗口阴影、圆角调节与内边距控制，适合制作教程插图或产品展示图。

### 🧹 智能消除与主体抠图
* **内容快速消除**：框选或涂抹截图中的隐私信息或杂乱背景，松手自动修补平整。
* **一键提取主体**：快速分离画面前景主体，支持仅复制抠图主体或一键转为透明贴图。

---

## ⌨️ 常用快捷键

| 功能 | 默认快捷键 | 操作说明 |
| :--- | :--- | :--- |
| **屏幕截图** | `⌥ + 1` (Option + 1) | 唤起截图，支持窗口智能边缘吸附 |
| **恢复上一张贴图** | `⌥ + 2` (Option + 2) | 从历史栈中重新打开最近关闭的贴图 |
| **截图历史记录** | `⌥ + 3` (Option + 3) | 浏览历史截图，支持本地离线搜索 |
| **快速 OCR 文字识别** | `⌥ + 4` (Option + 4) | 框选松手直接弹出文字识别结果 |
| **长截图** | `⌥ + 5` (Option + 5) | 框选区域后进入滚动拼接模式 |
| **动图录制 (GIF)** | `⌥ + 6` (Option + 6) | 录制指定区域的高清 GIF / MP4 动图 |
| **截图背景美化** | `⌥ + 7` (Option + 7) | 框选松手进入独立背景美化工作台 |
| **原地截图翻译 / 贴图翻译** | `⌥ + T` (Option + T) | 选区或贴图一键原地翻译 |
| **剪贴板转贴图** | `⌘ + ⌥ + T` | 复制文本、代码或图片后一键生成置顶贴图 |
| **贴图点击穿透** | `⌥ + G` (Option + G) | 切换贴图穿透模式，长按 `⌥` 可临时移动 |
| **标注单键直达** | `R` 矩形 / `A` 箭头 / `M` 马赛克 / `P` 画笔 / `L` 直线 / `T` 文本 / `N` 序号 / `B` 引线 / `W` 水印 | 在截图或贴图浏览状态下直接按单键开始标注 |

> 所有快捷键均可在「偏好设置」➔「快捷键」中自定义配置。

---

## 📥 下载与安装

1. 前往 GitHub [**Releases**](https://github.com/8wcznkmy6b-del/AuraSnap-PB/releases) 页面；
2. 下载最新版本 **`v3.0.16`** 的 `AuraSnap.app.zip`；
3. 解压后将 `AuraSnap.app` 拖入系统的 **应用程序 (Applications)** 文件夹；
4. 首次打开时，根据系统提示授予 **屏幕录制 (Screen Recording)** 与 **辅助功能 (Accessibility)** 权限即可正常使用。

---

## 🛡 隐私说明

AuraSnap 遵循本地优先原则：
* 屏幕截图、OCR 文字识别、长截图拼接与图像美化全部在 Mac 本地完成；
* 除非使用在线翻译功能，应用不会上传您的任何截图数据，确保个人与工作隐私安全。

---

## 💎 授权与 Pro 会员 (License & Pro Edition)

AuraSnap 采用 Freemium 模式，所有用户均可免费体验核心功能（包含每日免费 OCR、翻译与美化配额）。

升级 **Pro 会员** 解锁无限次极速原地翻译、长截图导出、高清录屏与高级美化模板：

* 🛒 **官方授权店铺**：[Creem Store (https://www.creem.io/stores/aurasnap)](https://www.creem.io/stores/aurasnap)
* 💳 **定价方案**：支持按年订阅（每月约 $0.83）与终生买断（$19.9 Lifetime）
* 🔑 **激活方式**：购买后获取授权激活码，在 App 菜单栏「偏好设置」➔「关于」中输入即可一键激活。

---

<div align="center">
  <sub>AuraSnap - Native screenshot toolkit for macOS.</sub><br>
  <sub>🌐 官方网站：<a href="https://aurasnap.dpdns.org/">https://aurasnap.dpdns.org/</a></sub>
</div>

