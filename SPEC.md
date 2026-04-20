# Personal Tech Blog - 科技博主个人站

## 设计理念
深色赛博极简风 — 沉稳的深黑底 + 霓虹绿点缀，营造沉浸式阅读氛围，大面积留白，克制但有科技感。

## 视觉方向
- 主色调：深黑 #0D0D0D + 霓虹绿 #00FF88
- 网格背景纹理，环境光晕效果
- 无衬线标题 + JetBrains Mono 等宽代码风格
- 极简卡片，无边框设计
- 滚动时文章卡片左侧霓虹边条出现

## 技术选型
- 单文件 HTML（零依赖，方便部署到任意静态托管）
- 原生 CSS + Vanilla JS
- Google Fonts: Space Grotesk (正文) + JetBrains Mono (等宽)
- localStorage 持久化存储文章数据

## 功能
- ✅ 文章列表页（首页）
- ✅ 文章详情页（点击后展开阅读）
- ✅ 响应式（手机/桌面）
- ✅ 发布管理面板（Ctrl+Shift+A 或点击「发布管理」唤起）
- ✅ 写文章（标题/日期/标签/摘要/正文）
- ✅ 编辑已有文章
- ✅ 删除文章
- ✅ localStorage 本地持久化（无需服务器）
- ✅ Toast 通知反馈

## 发布管理面板
- **唤起方式**：Ctrl+Shift+A 或点击右上角「✦ 发布管理」
- **关闭方式**：点击 ✕ 或按 Escape
- **写文章**：支持 HTML 标签（p, h2, h3, ul, li, blockquote, code, pre, strong）
- **数据存储**：localStorage，浏览器本地持久化，换设备需手动迁移

## 文章数据结构（localStorage）
```json
{
  "id": 1700000000000,
  "title": "文章标题",
  "date": "2024-03-15",
  "tags": ["效率", "工具"],
  "excerpt": "文章摘要...",
  "content": "<p>HTML 正文...</p>"
}
```

## 部署说明
将 `index.html` 上传至任意静态托管平台（GitHub Pages、Vercel、Netlify、Cloudflare Pages 等）即可上线。文章数据存储在用户浏览器 localStorage 中，网站本身无需服务器。
