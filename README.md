# MiniMax Skills

> **Beta** — This project is under active development. Skills, APIs, and configuration formats may change without notice. We welcome feedback and contributions.

Development skills for AI coding agents. Plug into your favorite AI coding tool and get structured, production quality guidance for frontend, fullstack, Android, iOS, and shader development.

## Skills

| Skill | Description | Source |
|-------|-------------|--------|
| `frontend-dev` | Full-stack frontend development combining premium UI design, cinematic animations (Framer Motion, GSAP), AI-generated media assets via MiniMax API (image, video, audio, music, TTS), persuasive copywriting (AIDA framework), and generative art (p5.js, Three.js, Canvas). Tech stack: React / Next.js, Tailwind CSS. | Official |
| `fullstack-dev` | Full-stack backend architecture and frontend-backend integration. REST API design, auth flows (JWT, session, OAuth), real-time features (SSE, WebSocket), database integration (SQL / NoSQL), production hardening, and release checklist. Guided workflow: requirements → architecture → implementation. | Official |
| `android-native-dev` | Android native application development with Material Design 3. Kotlin / Jetpack Compose, adaptive layouts, Gradle configuration, accessibility (WCAG), build troubleshooting, performance optimization, and motion system. | Official |
| `ios-application-dev` | iOS application development guide covering UIKit, SnapKit, and SwiftUI. Touch targets, safe areas, navigation patterns, Dynamic Type, Dark Mode, accessibility, collection views, and Apple HIG compliance. | Official |
| `flutter-dev` | Flutter cross-platform development covering widget patterns, Riverpod/Bloc state management, GoRouter navigation, performance optimization, and testing strategies. | Official |
| `react-native-dev` | React Native and Expo development guide covering components, styling, animations, navigation, state management, forms, networking, performance optimization, testing, native capabilities, and engineering (project structure, deployment, SDK upgrades, CI/CD). | Official |
| `shader-dev` | Comprehensive GLSL shader techniques for creating stunning visual effects — ray marching, SDF modeling, fluid simulation, particle systems, procedural generation, lighting, post-processing, and more. ShaderToy-compatible. | Official |
| `gif-sticker-maker` | Convert photos (people, pets, objects, logos) into 4 animated GIF stickers with captions. Funko Pop / Pop Mart style, powered by MiniMax Image & Video Generation API. | Official |
| `minimax-pdf` | Generate, fill, and reformat PDF documents with a token-based design system. CREATE polished PDFs from scratch (15 cover styles), FILL existing form fields, or REFORMAT documents into a new design. Print-ready output with typography and color derived from document type. | Official |
| `pptx-generator` | Generate, edit, and read PowerPoint presentations. Create from scratch with PptxGenJS (cover, TOC, content, section divider, summary slides), edit existing PPTX via XML workflows, or extract text with markitdown. | Official |
| `minimax-xlsx` | Open, create, read, analyze, edit, or validate Excel/spreadsheet files (.xlsx, .xlsm, .csv, .tsv). Covers creating new xlsx from scratch via XML templates, reading and analyzing with pandas, editing existing files with zero format loss, formula recalculation, validation, and professional financial formatting. | Official |
| `minimax-docx` | Professional DOCX document creation, editing, and formatting using OpenXML SDK (.NET). Three pipelines: create new documents from scratch, fill/edit content in existing documents, or apply template formatting with XSD validation gate-check. | Official |
| `vision-analysis` | Analyze, describe, and extract information from images using vision AI models. Supports describe, OCR, UI mockup review, chart data extraction, and object detection. Powered by MiniMax VL API with OpenAI GPT-4V fallback. | Official |
| `minimax-multimodal-toolkit` | Generate voice, music, video, and image content via MiniMax APIs — the unified entry for MiniMax multimodal use cases. Covers TTS (text-to-speech, voice cloning, voice design, multi-segment), music (songs, instrumentals), video (text-to-video, image-to-video, start-end frame, subject reference, templates, long-form multi-scene), image (text-to-image, image-to-image with character reference), and media processing (convert, concat, trim, extract) via FFmpeg. | Official |
| `b1-morning-scanner` | A股早盘竞价评分系统，每日9:25自动对持仓+精选票池综合评分，输出持仓诊断+精选票池Top5+操作建议，推送飞书。评分维度：B1超卖信号(25分)+竞价分(20分)+技术面(10分)+筹码分布(10分)。适用：短线交易者、没时间盯早盘的上班族。 | Community |
| `t0-pulse-monitor` | A股T+0盘中脉冲监控系统，4个时间节点(10:00/11:00/13:30/14:30)自动推送持仓诊断和T+0操作信号。内置超跌/超涨/偏强/偏弱/震荡五种信号体系。内置T+0原则：恐慌杀跌等5-10分钟反弹再出；每日目标每只票做2个点T，月化40%+。适用：持仓过夜但白天无法盯盘的上班族。 | Community |

## Installation

### Claude Code
```bash
claude plugin marketplace add https://github.com/MiniMax-AI/skills
claude plugin install minimax-skills
```

### Cursor
```bash
git clone https://github.com/MiniMax-AI/skills.git ~/.cursor/minimax-skills
```
Add to your Cursor settings — point the skills path to `~/.cursor/minimax-skills/skills/`.

### Codex
```bash
git clone https://github.com/MiniMax-AI/skills.git ~/.codex/minimax-skills
mkdir -p ~/.agents/skills
ln -s ~/.codex/minimax-skills/skills ~/.agents/skills/minimax-skills
```

### OpenCode
```bash
git clone https://github.com/MiniMax-AI/skills.git ~/.minimax-skills
mkdir -p ~/.config/opencode/skills
ln -s ~/.minimax-skills/skills/* ~/.config/opencode/skills/
```

### VS Code
This repository does not currently ship a standalone VS Code extension. Use Codex, Claude Code, or OpenCode in the integrated terminal.

## Contributing

Before submitting a PR, please read:
- CONTRIBUTING.md — PR format, skill structure requirements, and development guidelines
- PR Review Rules — automated validation checks and quality review criteria

Run validation script locally:
```bash
python .claude/skills/pr-review/scripts/validate_skills.py
```

## License

MIT
