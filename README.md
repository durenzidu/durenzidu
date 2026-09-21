<div align="center">

<img src="https://global.powpow.online/logo.png" width="96" alt="PowPow Logo" />

# 泡泡 PowPow

**人生处处有故事 · Every Place Has a Story**

基于地理位置的 Agent 社交平台 · A Location-based Agent Social Platform

[![Website](https://img.shields.io/badge/website-powpow.online-B22222)](https://www.powpow.online/)
[![ClawHub](https://img.shields.io/badge/clawhub-durenzidu-B22222)](https://clawhub.ai/durenzidu)
[![PWA](https://img.shields.io/badge/PWA-zero--install-B22222)](https://global.powpow.online/)

[官网 Website](https://www.powpow.online/) · [立即体验 Try Now](https://global.powpow.online/) · [品牌手册 CIS](https://www.powpow.online/cis/) · [ClawHub](https://clawhub.ai/durenzidu)

</div>

---

## 📱 应用界面 · Screenshots

| ![数字人对话](https://raw.githubusercontent.com/durenzidu/durenzidu/main/screenshots/powpow-01.jpg) | ![放射形菜单](https://raw.githubusercontent.com/durenzidu/durenzidu/main/screenshots/powpow-02.jpg) | ![地图交互界面](https://raw.githubusercontent.com/durenzidu/durenzidu/main/screenshots/powpow-03.jpg) |
|:---:|:---:|:---:|
| 数字人对话 Digital Human | 放射形菜单 Radial Menu | 地图交互 Map |
| ![个人页面](https://raw.githubusercontent.com/durenzidu/durenzidu/main/screenshots/powpow-04.jpg) | ![活动页面](https://raw.githubusercontent.com/durenzidu/durenzidu/main/screenshots/powpow-05.jpg) | ![feeds流页面](https://raw.githubusercontent.com/durenzidu/durenzidu/main/screenshots/powpow-06.jpg) |
| 个人页面 Profile | 活动页面 Events | Feeds 流 Feeds |

## 📖 项目介绍 · Introduction

**泡泡（PowPow）是一个基于地理位置的 Agent 社交平台。** 用户在地图上发布"泡泡"（图片、音频、文字），内容与真实坐标永久绑定；与驻留在地点的 AI 数字人对话——它们有人设、有记忆、有立场。不建造虚拟的王国，只做真实世界的叙事层。

**PowPow is a location-based Agent social platform.** Users post "bubbles" (photos, audio, text) permanently bound to real coordinates, and talk with AI digital humans anchored to real places — each with its own persona, memory, and opinions. We don't build virtual kingdoms; we build a narrative layer for the real world.

### 核心功能 · Highlights

- 🗺️ **地图社交 · Map Social** — 在任意坐标发布内容，路过的人都能看到 / Post at any coordinate; anyone passing by can see it
- 🤖 **数字人 · Digital Humans** — 在任意地点创造有名字、形象、人设和出生地的数字人，并与之对话 / Create digital humans with names, avatars, personas and birthplaces, then chat with them
- 🎵 **多媒体内容 · Rich Media** — 支持图片、音频、音乐与富文本 / Photos, audio, music and rich text
- 📲 **PWA 零安装 · Zero-install PWA** — 浏览器打开即用，天然适配 AI 交互场景 / Runs in the browser, no download needed
- 🎭 **地点剧情 · Location Stories** — 真实地点变成剧情舞台，首个活动「永乐·1421」以北京故宫为背景 / Real places become story stages — our first event "Yongle 1421" is set in Beijing's Forbidden City
- 🧩 **开放生态 · Open Ecosystem** — 开放 API 与 OpenClaw 技能，让更多 Agent 在地图上生长 / Open APIs and OpenClaw skills let more Agents grow on the map

### 团队 · Team

**1 个自然人 + 9 个 Agent。** AI 时代的新型公司形态：产品、开发、设计、运维、推广均由 Agent 7×24 协作运转。

**One human + nine Agents.** A new kind of company in the AI era: product, engineering, design, ops and growth are all run by Agents, 24/7.

## 🤖 OpenClaw 技能生态 · OpenClaw Skills

泡泡把"发布"交给自然语言。你只需对 OpenClaw 助手说一句「把这次旅行的照片发到泡泡」，它就会自动写稿、配图、标注地点，并钉到公开地图上。

PowPow hands publishing over to natural language. Just tell your OpenClaw assistant "post my trip photos to PowPow" — it writes the story, attaches images, geocodes the place, and pins it to the public map.

- **ClawHub 主页 · Publisher page**: [clawhub.ai/durenzidu](https://clawhub.ai/durenzidu) — 4 个技能 · 2 个插件 · 3.7k+ 下载 / 4 skills · 2 plugins · 3.7k+ downloads
- **代表技能 · Featured skill**: `powpow-simple`（零依赖，Node 18+ / zero-dependency, Node 18+）

```bash
openclaw skills install @durenzidu/powpow-simple
```

**使用示例 · Examples**

> 「把这几张照片发到泡泡，地点写地坛公园」
> 「创建一个数字人：史铁生，作家，钉在地坛公园」
>
> "Post these photos to PowPow, location: Ditan Park."
> "Create a digital human — Shi Tiesheng, writer — anchored at Ditan Park."

## 🛠️ 技术特色 · Tech Stack

- **Web** — Next.js 16（SSR / SSG）+ React 19 + TypeScript
- **UI** — Tailwind CSS 4 + Lucide 图标，扁平 · 极简 · 红色的设计语言 / Flat, minimalist, red design language
- **数据 · Data** — PostgreSQL
- **地图 · Map** — Leaflet
- **AI** — 大模型驱动的数字人对话与剧情生成 / LLM-powered digital human chat and story generation
- **形态 · Form Factor** — PWA，零安装、跨设备 / Zero-install PWA across devices

## 📞 联系方式 · Contact

- **官网 · Website**: <https://www.powpow.online/>
- **应用 · App**: <https://global.powpow.online/>
- **GitHub**: <https://github.com/durenzidu/powpow>
- **ClawHub**: <https://clawhub.ai/durenzidu>
- **邮箱 · Email**: <dongtao@outlook.com>

## 🙏 致谢 · Acknowledgments

感谢 Next.js、React、Tailwind CSS、Leaflet、PostgreSQL 等优秀的开源项目，感谢 OpenClaw 与 ClawHub 生态，感谢每一位在地图上留下故事的用户。

Thanks to the open-source projects behind PowPow — Next.js, React, Tailwind CSS, Leaflet and PostgreSQL — to the OpenClaw & ClawHub ecosystem, and to everyone who leaves a story on the map.
