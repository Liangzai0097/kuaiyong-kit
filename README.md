# 快用工具箱（kuaiyong-kit）

免费、安全、无需注册的在线小工具集合。所有工具在浏览器本地运行，文件不上传服务器。

## 当前工具

- 🖼️ 图片压缩 (`tools/image-compress.html`) — 支持 JPG/PNG/WebP，可调质量与尺寸

## 技术栈

纯静态站，零依赖：HTML + CSS + 原生 JavaScript。

## 本地预览

任意静态服务器即可，例如：

```bash
# Python
python3 -m http.server 8080

# 或 Node
npx serve .
```

然后访问 http://localhost:8080。

## 部署（GitHub Pages）

1. 在 GitHub 新建仓库，例如 `kuaiyong-kit`。
2. 在本地目录初始化并推送：
   ```bash
   git init
   git add .
   git commit -m "init: 项目骨架 + 图片压缩工具"
   git branch -M main
   git remote add origin git@github.com:<你的用户名>/kuaiyong-kit.git
   git push -u origin main
   ```
3. 仓库 → Settings → Pages → Source 选 `Deploy from a branch`，分支选 `main`，目录选 `/ (root)`，保存。
4. 等 1-2 分钟，访问 `https://<你的用户名>.github.io/kuaiyong-kit/`。

## 上线后建议（零成本能做的）

- 把 `index.html`、`tools/image-compress.html`、`sitemap.xml`、`robots.txt` 中的 `https://example.github.io/` 替换成你的真实地址。
- 提交到 [Bing 站长](https://www.bing.com/webmasters/) 和 [Google Search Console](https://search.google.com/search-console)。
- 百度对 `github.io` 抓取很差，等做 ICP 备案 + 自有域名后再提交百度。

## 阶段计划

- **阶段 1（当前，0 成本）**：在 GitHub Pages 上跑 1-2 周，验证流程，看 Bing/Google 收录。
- **阶段 2（决定是否投入）**：如果觉得值得，再买 `.cn` 域名（约 38 元/年）+ 阿里云轻量服务器（约 99 元/年）+ ICP 备案，做百度 SEO。
