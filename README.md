# Blog

简体中文 · 一个基于 JavaScript/EJS 的个人博客项目。

## 介绍
这是我的个人博客仓库，用于写作、展示和记录个人项目与心得。项目使用服务端渲染模板（EJS）构建页面，前端使用 JavaScript 与 CSS 实现交互与样式。

## 技术栈
- 语言：JavaScript, EJS, HTML, CSS
- 模板引擎：EJS
- 运行环境：Node.js
- 静态资源：public/（CSS、JS、图片等）

仓库语言构成（近似）：
- JavaScript ~39.6%
- CSS ~25.4%
- EJS ~22.5%
- HTML ~12.5%

## 功能（示例）
- 文章列表与单篇展示
- 基本的路由与页面模板
- 可扩展的静态资源结构（CSS/JS）
- 支持添加评论/标签（视实现而定）

## 快速开始
先确保已安装 Node.js 与 npm/yarn。

1. 克隆仓库
   git clone https://github.com/username-wzy/blog.git
2. 进入项目目录
   cd blog
3. 安装依赖
   npm install
   或
   yarn
4. 运行项目（开发模式）
   npm start
   或
   NODE_ENV=development npm run dev

默认会在本地的 3000 端口启动（若项目中有指定 PORT 环境变量，请按项目要求设置）。

## 配置
在根目录创建 `.env`（若项目使用环境变量）并配置常用项，例如：
- PORT=3000
- DATABASE_URL=（如使用数据库）
- SESSION_SECRET=（如使用会话）

具体配置项以项目代码中的说明或示例文件为准（如 `.env.example`）。

## 目录结构（示例）
- /views — EJS 模板
- /public — 静态资源（CSS、JS、images）
- /routes — 路由（若有）
- /controllers — 逻辑处理（若有）
- /models — 数据模型（若有）
- app.js / index.js — 入口文件

根据仓库实际结构调整。

## 开发建议
- 在本地使用 nodemon 提高开发效率（npm i -D nodemon）
- 将可配置项移入环境变量，不要在仓库中提交敏感信息
- 将发布/部署脚本写入 package.json 的 scripts 中

## 部署
可部署到任意支持 Node.js 的平台（例如：Vercel、Heroku、Render、传统 VPS）。部署步骤通常为：
- 安装依赖：npm install
- 构建（如有构建步骤）
- 启动：npm start
- 配置环境变量（PORT、数据库连接等）