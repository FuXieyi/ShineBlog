# 特别感谢saicaca
此项目原始模版是基于此作者的fuwari
https://github.com/saicaca/fuwari

# 🌟 Shine - 简约静态博客模板

一个基于Astro构建的现代静态博客模板,界面简洁,功能丰富。

**🖥️ [在线演示](https://your-demo-site-url.com)** / **📦 [源代码](https://github.com/your-username/shine)**

> README版本: `2025-06-01`

## ✨ 特性

* 基于Astro和Tailwind CSS构建
* 流畅的页面过渡和动画效果
* 支持亮色/暗色模式
* 自定义主题色彩和横幅
* 完全响应式设计
* 支持数学公式(KaTeX)
* 表格内容(TOC)自动生成
* 文章搜索功能
* 多语言支持(中文、英文等)
* 标签和分类系统
* 自定义Markdown扩展功能

## 📋 系统要求

* Node.js >= 18
* pnpm >= 9

## 🚀 使用方法

1. 从此模板生成新仓库或fork此仓库
2. 克隆您的仓库到本地
3. 安装依赖:
   ```bash
   pnpm install
   pnpm add sharp
   ```
   * 如果尚未安装pnpm,请先运行 `npm install -g pnpm`
4. 在`src/config.ts`中自定义您的博客设置
5. 运行`pnpm dev`启动本地开发服务器
6. 使用`pnpm new-post <文件名>`创建新文章,并在`src/content/posts/`中编辑

## ⚙️ 文章frontmatter配置

```yaml
---
title: 我的第一篇博客文章
published: 2023-09-09
updated: 2023-09-09
description: 这是我的Astro博客的第一篇文章。
image: ./cover.jpg
tags: [前端, Astro, 博客]
category: Web开发
draft: false
lang: zh_CN  # 仅当文章语言与config.ts中设置的站点语言不同时设置
---
```

## 📝 自定义配置

在`src/config.ts`中,您可以配置:

- 网站标题和副标题
- 网站语言
- 主题色调
- 横幅设置和图片
- 目录显示选项
- 网站图标(favicon)
- 导航栏链接
- 个人资料信息
- 许可证信息

## 🧞 常用命令

所有命令都在项目根目录下的终端中运行:

| 命令                          | 操作                           |
| ----------------------------- | ------------------------------ |
| `pnpm install && pnpm add sharp` | 安装依赖                       |
| `pnpm dev`                    | 在localhost:4321启动本地开发服务器 |
| `pnpm build`                  | 构建生产站点到./dist/目录      |
| `pnpm preview`                | 在部署前本地预览构建结果       |
| `pnpm new-post <文件名>`      | 创建新文章                     |
| `pnpm astro ...`              | 运行Astro CLI命令              |
| `pnpm astro --help`           | 获取Astro CLI帮助              |

## 📚 Markdown扩展功能

本模板支持多种Markdown扩展功能:

### 数学公式

```markdown
行内公式: $\omega = d\phi / dt$

独立公式:
$$I = \int \rho R^{2} dV$$
```

### 提示框

```markdown
::: note
这是一个笔记提示框
:::

::: tip
这是一个提示框
:::

::: warning
这是一个警告框
:::

::: caution
这是一个注意框
:::
```

## 🌐 部署

在部署之前,请编辑`astro.config.mjs`中的站点配置:

```javascript
export default defineConfig({
  site: "https://你的网站域名.com",
  // ...
});
```

然后可以部署到:
- Vercel
- Netlify
- GitHub Pages
- 或其他静态网站托管服务

## 📜 许可证

MIT License

## 🙏 致谢

- [Astro](https://astro.build/)
- [Tailwind CSS](https://tailwindcss.com/)
- [Svelte](https://svelte.dev/)
- 所有开源贡献者

---

如有问题或建议,欢迎提交Issue或Pull Request。

[⬆ 返回顶部](#-shine---简约静态博客模板) 