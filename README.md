# Roleplay Hub

Roleplay Hub 是一个纯前端运行的本地优先 AI Roleplay 对话和角色卡工具。本仓库基于 [STA1N156/RP-Hub](https://github.com/STA1N156/RP-Hub) 部署整理，并保留原项目的非商业授权要求。

## 功能概览

- AI Roleplay 对话与上下文管理
- 角色卡导入、编辑与导出
- 角色卡工坊：`/character/`
- OpenAI 兼容 API 配置
- 浏览器本地存储，默认不需要后端服务

## 快速开始

直接双击 `index.html` 通常即可使用。更推荐使用本地静态服务预览：

```powershell
python -m http.server 5173
```

然后访问：

```text
http://localhost:5173/
```

## 部署

仓库已包含 GitHub Pages 自动部署工作流：`.github/workflows/pages.yml`。

详细步骤见 [DEPLOYMENT.md](./DEPLOYMENT.md)。

## 目录结构

```text
Roleplay-Hub/
├── index.html
├── character/
│   └── index.html
├── assets/
│   ├── css/
│   │   └── styles.css
│   ├── js/
│   │   ├── app.js
│   │   ├── card-utils.js
│   │   ├── ui-select.js
│   │   └── utils.js
│   └── favicon.svg
├── site.webmanifest
├── DEPLOYMENT.md
└── LICENSE
```

## 授权

本项目遵循 [Creative Commons Attribution-NonCommercial 4.0 International](./LICENSE) 协议。

你可以自由分享和修改，但必须署名，且不得用于商业用途。
