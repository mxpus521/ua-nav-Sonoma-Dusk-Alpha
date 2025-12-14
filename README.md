# WebNav Hub 🌐

![Version](https://img.shields.io/badge/version-1.0.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Status](https://img.shields.io/badge/status-active-success)

**WebNav Hub** 是一个精心打造的综合性网页导航中心，旨在为用户提供从人工智能前沿工具到日常实用软件的一站式访问入口。

该项目采用极简而现代的设计语言，结合醒目的蓝黄配色，不仅在视觉上令人耳目一新，更在交互上追求极致的流畅体验。无论您是科技爱好者、创意工作者还是日常互联网用户，WebNav Hub 都能帮助您高效管理和发现网络资源。

---

## ✨ 核心特性

-   **🎨 现代美学设计**
    -   采用 **蓝与黄** 的高对比度配色方案（灵感源自乌克兰国旗配色），视觉冲击力强且清晰易读。
    -   全站应用 **CSS3 阴影与过渡动画**，卡片悬停时有灵动的上浮与旋转微交互。

-   **📱 全终端响应式**
    -   **桌面端**：宽屏展示，网格布局充分利用空间。
    -   **移动端**：自适应单列或双列布局，针对触摸操作优化了点击区域。
    -   完美支持从 4k 大屏到 iPhone SE 等小屏设备的无缝切换。

-   **🚀 流畅交互体验**
    -   **顶部悬浮导航**：导航栏始终吸顶，支持锚点平滑滚动定位。
    -   **智能高亮**：滚动页面时，导航菜单会自动高亮显示当前所在的版块。
    -   **无刷新体验**：点击分类时 URL 哈希平滑更新，支持浏览器后退功能。

-   **📂 丰富资源分类**
    -   覆盖 **Ai 搜索**、**社交媒体**、**实用工具**、**科技资讯**、**云存储**、**电子邮箱** 等六大核心领域。

---

## 🛠️ 技术架构

本项目坚持 **"回归原生，极致轻量"** 的开发理念，不依赖庞大的前端框架，确保页面秒开：

| 技术 | 描述 |
| :--- | :--- |
| **HTML5** | 语义化标签构建（`<main>`, `<section>`, `<nav>`），利于 SEO 和无障碍访问。 |
| **CSS3** | 使用 **CSS Variables (:root)** 管理主题，**Flexbox & Grid** 处理复杂布局。 |
| **JavaScript** | 原生 ES6+，无 jQuery 依赖。实现 `IntersectionObserver` 类似的滚动监听逻辑。 |
| **FontAwesome** | 引入 `FontAwesome 6` 矢量图标库，提供高清、可缩放的视觉图标。 |

---

## 📂 目录结构

```text
/mv
├── index.html      # 核心入口文件，包含所有 DOM 结构和链接数据
├── styles.css      # 样式表，定义主题变量、响应式规则和动画
├── script.js       # 交互逻辑，处理滚动监听、高亮和路由哈希
└── README.md       # 项目说明文档
```

---

## 🚀 快速开始

无需 `npm install`，无需构建步骤，即开即用。

### 本地运行

1.  **获取代码**
    ```bash
    git clone https://github.com/yourusername/webnav-hub.git
    # 或者直接下载 ZIP 压缩包
    ```

2.  **启动**
    -   直接双击文件夹中的 `index.html`，即可在浏览器中预览。
    -   (可选) 使用 VS Code 的 "Live Server" 插件运行，体验更佳。

### 部署上线

由于本项目是纯静态网页，您可以轻松将其免费部署到以下平台：

-   **GitHub Pages**: 上传代码到 GitHub 仓库，在 Settings -> Pages 中开启即可。
-   **Vercel / Netlify**: 直接导入 GitHub 仓库，无需配置构建命令（Build Command 留空）。

---

## 🎨 自定义指南

想要添加自己的常用链接？非常简单！

### 1. 添加新链接卡片
打开 `index.html`，定位到您想添加的分类（例如 `#tools`），复制以下模板代码：

```html
<div class="link-card">
  <!-- 替换 href 为目标网址 -->
  <a href="https://example.com" target="_blank"></a>
  <!-- 替换 class 为 FontAwesome 图标，例如 fa-solid fa-code -->
  <i class="fa-solid fa-star"></i>
  <!-- 填写显示的标题 -->
  <h3>我的新网站</h3>
</div>
```

### 2. 修改主题颜色
打开 `styles.css`，在文件顶部的 `:root` 区域修改变量即可全局换肤：

```css
:root {
  --primary-color: #ffd500; /* 主色调 (文字、图标、高亮) */
  --bg-color: #005bbb;      /* 页面背景色 */
  --card-bg-color: #004a99; /* 卡片背景色 */
  /* ... */
}
```

---

## 🤝 贡献与支持

如果您发现链接失效或有更好的设计建议，欢迎提交 **Pull Request** 或 **Issue**。

1.  Fork 本仓库
2.  新建分支 `git checkout -b feature/AmazingFeature`
3.  提交更改 `git commit -m 'Add some AmazingFeature'`
4.  推送到分支 `git push origin feature/AmazingFeature`
5.  提交 Pull Request

## � 许可证

本项目基于 MIT 许可证开源 - 详情请参阅 [LICENSE](LICENSE) 文件（如有）。

---

<p align="center">Made with ❤️ by WebNav Team</p>
