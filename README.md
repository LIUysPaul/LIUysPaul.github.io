# LIUysPaul.github.io

> 个人主页 · Personal Homepage

基于 GitHub Pages 搭建的个人静态主页，使用纯 HTML + CSS 实现，无需任何构建工具。

## ✨ Features

- 🎨 **极简设计** - 深色主题，干净简约的视觉风格
- 📱 **响应式布局** - 完美适配桌面端与移动端
- 🗂️ **项目展示** - 卡片式网格展示 GitHub 仓库
- 📊 **数据统计** - About 区域展示项目概览数据
- 🔗 **社交链接** - Footer 集成 GitHub、邮箱等联系方式
- ⚡ **零依赖** - 纯原生 HTML/CSS，加载速度快

## 📁 Project Structure

```
.
├── index.html          # 主页文件（含所有样式）
├── README.md           # 项目说明文档
├── motorcycle.png      # 旧图片（已弃用）
└── files/              # 其他资源文件
```

## 🚀 Usage

### 本地预览

直接用浏览器打开 `index.html` 即可：

```bash
# macOS
open index.html

# Linux
xdg-open index.html
```

或者启动一个简单的本地 HTTP 服务器：

```bash
# Python 3
python3 -m http.server 8000

# Node.js (需全局安装 serve)
npx serve .
```

然后访问 `http://localhost:8000`。

### 部署到 GitHub Pages

1. 将代码推送到你的 GitHub 仓库（仓库名需为 `<username>.github.io`）
2. 进入仓库 Settings → Pages
3. Source 选择 `main` 分支，根目录 `/`
4. 保存后访问 `https://<username>.github.io`

## 🎯 Customization

### 修改个人信息

在 `index.html` 中搜索以下内容并替换：

- **姓名 / 标题**: `<h1>LIU Y.</h1>` 和 `<title>LIU Y. | Homepage</title>`
- **副标题**: `<p class="subtitle">Developer · Creator · Builder</p>`
- **GitHub 链接**: 所有 `https://github.com/LIUysPaul` 替换为你的地址
- **邮箱**: `mailto:your@email.com` 替换为你的邮箱

### 添加仓库卡片

找到 `<section class="projects">` 区域，复制并修改以下模板：

```html
<div class="project-card">
  <div class="project-icon">🚀</div>
  <h3 class="project-name">仓库名称</h3>
  <p class="project-desc">仓库的简短描述...</p>
  <div class="project-meta">
    <div class="project-lang">
      <span class="lang-dot" style="background: #e34c26;"></span>
      语言名称
    </div>
    <a href="https://github.com/你的用户名/仓库名" target="_blank" class="project-link">查看 →</a>
  </div>
</div>
```

语言颜色参考：
- HTML: `#e34c26`
- CSS: `#563d7c`
- JavaScript: `#f1e05a`
- TypeScript: `#3178c6`
- Python: `#3572A5`
- Go: `#00ADD8`
- Rust: `#dea584`
- Java: `#b07219`
- Vue: `#41b883`
- React/JSX: `#61dafb`

### 修改统计数据

找到 `<section id="about">` 中的 `.stats-grid`，修改数字和标签即可。

### 修改主题颜色

在 CSS 中搜索以下颜色值进行调整：

- 主背景: `#0a0a0a`
- 次级背景: `#0d0d0d` / `#111`
- 主文字: `#e5e5e5`
- 次要文字: `#787878` / `#6b7280`

## 📄 License

MIT License - feel free to use this template for your own homepage.

---

© 2026 LIU Y. Built with ❤️ and pure HTML/CSS.
