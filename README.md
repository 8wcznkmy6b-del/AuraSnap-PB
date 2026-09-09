<div align="center">
  <img src="https://raw.githubusercontent.com/8wcznkmy6b-del/AuraSnap-PB/main/AuraSnap.png?v=2" width="120" alt="AuraSnap Icon" />
  <h1>AuraSnap</h1>
  <p>专为 macOS 打造的原生截图与系统级效率工具箱</p>
  <p>集截图翻译、屏幕贴图、径向分屏、鼠标外设增强、多云图床直传与访达超级右键于一体。</p>
  <p>
    <a href="https://aurasnap.dpdns.org/"><img src="https://img.shields.io/badge/官网-aurasnap.dpdns.org-0ea5e9?style=flat-square&logo=safari" alt="Website" /></a>
    <a href="https://github.com/8wcznkmy6b-del/AuraSnap-PB/releases"><img src="https://img.shields.io/badge/最新版本-v3.0.57-10b981?style=flat-square&logo=apple" alt="Release" /></a>
    <img src="https://img.shields.io/badge/macOS-14.0+-blue?style=flat-square" alt="macOS" />
    <img src="https://img.shields.io/badge/架构-Apple_Silicon_原生-purple?style=flat-square" alt="Apple Silicon" />
  </p>
  <p>
    <a href="README.md"><b>简体中文</b></a> | <a href="README_EN.md"><b>English</b></a>
  </p>
</div>

---

## 💡 产品简介

**AuraSnap** 是一款纯 Swift 原生开发的 macOS 深度系统级效率工具。摒弃了 Electron 的臃肿和高能耗，日常驻留内存通常小于 **40MB**。

它不仅具备像素级截图标注、AI 原地排版翻译、屏幕置顶贴图与平滑长截图，更深度整合了 **Liquid Glass 径向分屏轮盘**、**鼠标外设多方案增强**、**原生 10 大云存储图床** 与 **访达 (Finder) 超级右键扩展**，让你用一个轻盈的原生 App，替代数个同类常驻软件。

---

## ✨ 核心功能全览

### 🪟 径向分屏管理 (Radial Window Manager)
* **Apple Liquid Glass 液态玻璃材质**：四款轮盘形态均支持原生液态玻璃通透折射，呼出时不抢占前台输入焦点，视觉高级且克制。
* **全新「引力透镜」主题**：无接缝一体化圆盘设计，罗盘式微光向量针平滑追随光标转向，中心区域实时显示 1:1 屏幕布局拓扑。
* **微晶底色与独立高亮流光定制**：提供 7 款微晶底色与 8 款独立高亮流光色相，通透度支持自由微调，并配备 1:1 真实光标手势动态仿真实验台。
* **8 向极速径向吸附与智能补位**：按住滚轮中键、侧键或修饰键轻推鼠标，秒级吸附至左右半屏、上下半屏、四角 1/4、居中或全屏；具备智能邻接贴合与台前调度安全区避让。

### 🖱️ 鼠标外设全维度增强 (Mouse & Input Enhancer)
* **多鼠标 Profile 独立管理与硬件感知**：支持为办公、游戏、便携等不同鼠标独立维护按键映射方案；内置 `DeviceMatcher` 基于厂商 ID、产品 ID 与物理序列号自动识别接入的鼠标，插拔时自动无缝切换对应方案，并显示连接状态胶囊（🟢/🟠/⚪️）。
* **「按住此键 + 滚动滚轮」多任务手势联动**：
  * 按住指定侧键（或中键）并滑动滚轮，滚轮事件被手势引擎平滑接管；
  * 支持 **平滑切换全屏桌面 (Spaces)**、**快速循环切应用 (⌘Tab)**、**切换同应用窗口 (⌘`)**、**切换标签页** 与 **画布无级缩放**；
  * 配备精准状态机防误触：转动滚轮后松开按键，自动阻断单击动作。
* **模拟触控板平滑滚动与应用例外名单**：将机械滚轮离散阶跃转化为触控板级惯性平滑；可自主为特定专业软件添加白名单，放行原生硬件信号。
* **独立反转与线性指针**：独立反转外接鼠标滚轮方向，内置触控板不受影响；消除系统非线性加速度，实现 1:1 像素级跟手。

### ☁️ 原生图床与云存储直传 (Image Hosting & Cloud Upload)
* **支持 10 大主流云存储生态**：
  * **S3 协议生态**：Amazon S3、Cloudflare R2、MinIO (自建私有云)、Backblaze B2、DigitalOcean Spaces、腾讯云 COS (S3 兼容)；
  * **国内专有协议**：阿里云 OSS、七牛云 KODO；
  * **极客与版本控制**：GitHub 仓库直传、自定义 Webhook / HTTP POST API。
* **格式智能转换与压缩**：支持 WebP、JPEG、PNG 多格式即时编码导出与质量滑块控制。
* **AI 智能命名与自动回填**：截图保存时可调用大模型语义理解画面内容自动生成文件名；上传完成后自动写入剪贴板（支持 Markdown、HTML、纯 URL 等格式），伴随轻盈 Toast 提示。

### 📁 访达超级右键 (FinderSync Extension)
* **系统原生风格单层菜单**：基于原生 `FinderSync` 独立扩展进程架构运行，移除冗余彩色图标，深度契合 macOS 视觉规范，极速稳定不卡死。
* **空白处一键新建文件**：内置十余种常用模板（Office 文档、Markdown 笔记、JSON/YAML/Shell/Python/Swift 等代码文件及 `.env`、`.gitignore`），支持自定义模板目录与工程脚手架。
* **扁平化目录操作**：简化“拷贝到”和“移动到”的操作层级，直接唤起系统目录选择器；支持跨卷移动与完成即时高亮定位。
* **路径快速提取**：一键复制 POSIX 绝对路径、Shell 终端转义路径或 URL 链接至剪贴板，随处粘贴无障碍。

### 🌐 AI 原地排版翻译 (In-Place Translation)
* **原地擦除与排版重绘**：框选外文区域，直接在原图对应位置擦除背景并重新绘制译文；自动继承源图基线高度、字重字阶与文本色彩，保留原始段落版式。
* **多服务商接入**：内置免费配置的快捷通道，同时支持配置 DeepL、Google Cloud、Azure、百度、腾讯、火山引擎等标准服务。
* **贴图即时对照**：置顶悬浮贴图支持右键即时翻译与双语原文对照。

### 📌 屏幕贴图与手势交互 (Floating Pins)
* **置顶悬浮与 120Hz 视网膜缩放**：一键将截图、纯文本或剪贴板图片固定在屏幕顶层，双指捏合或滚轮平滑缩放。
* **⌘ 键直接拖拽外发**：按住 `Command` 拖拽贴图，可直接拖入微信、飞书、邮件或访达保存。
* **幽灵穿透模式 (Ghost Mode)**：开启穿透后鼠标可直接穿透贴图操作底层内容；长按 `Option` 可临时移动。

### 📜 工业级平滑长截图 (Scrolling Capture)
* **双引擎自适应拼接**：基于 Apple Accelerate 硬件级矢量加速与 vDSP 算法，支持网页、代码、终端长日志平滑滚动实时拼接，带右侧实时预览图，有效过滤悬停表头与固底栏。

### 🔍 离线文字识别 (OCR)
* **Apple Vision 原生引擎**：秒级离线多语言高精度识别；智能识别段落排版与表格结构，支持一键导出为标准 Markdown 表格。

### 🎨 截图背景美化与光影工作台
* **社媒分享卡片一键生成**：智能提取主色调生成莫兰迪渐变背景，或直接使用系统 5K 桌面壁纸作为衬底。
* **拟真光影与落影治理**：自适应 macOS 原生窗口阴影与圆角，两阶段物理像素直通管线彻底杜绝带阴影复制时的标注位移缺陷。

---

## ⌨️ 常用快捷键一览

| 功能 | 默认快捷键 | 操作说明 |
| :--- | :--- | :--- |
| **屏幕截图** | `⌥ + 1` (Option + 1) | 唤起截图，支持智能窗口探测与边缘吸附 |
| **恢复上一张贴图** | `⌥ + 2` (Option + 2) | 从历史栈中重新打开最近关闭的贴图 |
| **截图历史画廊** | `⌥ + 3` (Option + 3) | 浏览历史截图记录，支持本地搜索 |
| **快速 OCR 识别** | `⌥ + 4` (Option + 4) | 框选松手直接提取文字，支持复制为 Markdown |
| **长截图** | `⌥ + 5` (Option + 5) | 框选区域后进入平滑滚动拼接模式 |
| **动图录制 (GIF)** | `⌥ + 6` (Option + 6) | 录制指定区域的高清 GIF / MP4 动图 |
| **截图背景美化** | `⌥ + 7` (Option + 7) | 框选进入独立美化工作台，生成带背景展示图 |
| **原地截图 / 贴图翻译** | `⌥ + T` (Option + T) | 选区或贴图一键原地排版翻译 |
| **分屏管理 (手势轮盘)** | 按住滚轮 / 侧键 / `Fn` / `⌥` 滑动 | 唤起 8 向液态玻璃轮盘，轻推松手秒级吸附 |
| **窗口半屏分屏** | `⌃ + ⌥ + ←` / `→` / `↑` / `↓` | 将前台窗口吸附至 左 / 右 / 上 / 下 半屏 (50%) |
| **全屏最大化 / 居中窗口** | `⌃ + ⌥ + ↩` / `C` | 全屏铺满当前屏幕 / 居中显示窗口 |
| **四角 1/4 分屏** | `⌃ + ⌥ + U` / `I` / `J` / `K` | 吸附至 左上 / 右上 / 左下 / 右下 1/4 区域 |
| **剪贴板转贴图** | `⌘ + ⌥ + T` | 复制文本、代码或图片后一键生成置顶贴图 |
| **贴图点击穿透** | `⌥ + G` (Option + G) | 切换贴图穿透模式，长按 `⌥` 可临时移动 |
| **快捷上传至图床** | `⌥ + U` (Option + U) | 将选区截图直接上传至默认配置的图床服务 |

> 💡 **全局快捷键独立解耦**：所有全局快捷键均在「偏好设置」➔「快捷键」中提供**独立开关**。未启用的快捷键会彻底注销监听，自动放行给 Final Cut Pro、Xcode、Photoshop 等专业软件使用，绝不冲突。

---

## 📥 下载与安装

1. 前往 GitHub [**Releases**](https://github.com/8wcznkmy6b-del/AuraSnap-PB/releases) 页面；
2. 下载最新版本 **`v3.0.57`** 的 `AuraSnap.dmg` 或 `AuraSnap.app.zip`；
3. 将 `AuraSnap.app` 拖入系统的 **应用程序 (Applications)** 文件夹；
4. 首次打开时，根据系统引导授予 **屏幕录制 (Screen Recording)** 与 **辅助功能 (Accessibility)** 权限即可开启体验。

---

## 🛡 隐私说明与本地优先

AuraSnap 严格恪守 **Local-First（本地优先）** 准则：
* 屏幕截图、标注排版、OCR 文字识别、长截图拼接、分屏管理、鼠标拦截与访达操作 **100% 运行在 Mac 本地**；
* 除用户主动发起的在线翻译请求或图床直传外，应用绝不上传任何屏幕数据与操作隐私，安全纯净。

---

## 💎 授权与 Pro 会员 (License & Pro Edition)

AuraSnap 采用 Freemium 模式，所有基础用户均可免费体验核心功能。

升级 **Pro 会员** 解锁无限次极速原地翻译、长截图无损导出、高清动图录制、多图床无缝直传与高级美化模板：

* 🛒 **官方授权店铺**：[Creem Store (https://www.creem.io/stores/aurasnap)](https://www.creem.io/stores/aurasnap)
* 💳 **定价方案**：支持按年订阅（每月约 $0.83）与终生买断（$19.9 Lifetime）
* 🔑 **激活方式**：购买后在 App 菜单栏「偏好设置」➔「关于」中输入授权码即可秒级激活。

---

<div align="center">
  <sub>AuraSnap - Native All-in-One Productivity & Screenshot Toolkit for macOS.</sub><br>
  <sub>🌐 官方网站：<a href="https://aurasnap.dpdns.org/">https://aurasnap.dpdns.org/</a></sub>
</div>
