# 部署说明

这个仓库是纯前端静态应用，不需要 Node.js 构建步骤。你可以直接用 GitHub Pages 部署。

## GitHub Pages 自动部署

1. 在 GitHub 创建你自己的仓库。
2. 把本地代码推送到该仓库的 `main` 分支。
3. 打开仓库的 `Settings` -> `Pages`。
4. 在 `Build and deployment` 里选择 `GitHub Actions`。
5. 推送后等待 `Deploy to GitHub Pages` 工作流完成。

部署完成后，Pages 页面会显示公开访问地址。应用数据和 API Key 存在浏览器本地，请不要把个人配置写入仓库。

## 本地预览

在仓库根目录运行：

```powershell
python -m http.server 5173
```

然后打开：

```text
http://localhost:5173/
```

角色卡工坊位于：

```text
http://localhost:5173/character/
```

## 注意事项

- 本项目基于 `CC BY-NC 4.0` 协议，不能用于商业用途。
- 页面依赖 Vue、Tailwind、Marked、DOMPurify 等 CDN 资源，离线环境下首次加载可能不可用。
- 如 API 提供商不允许浏览器跨域请求，需要换用支持 CORS 的兼容接口或自建代理。
