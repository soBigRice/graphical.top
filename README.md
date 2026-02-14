# graphical.top Homepage

一个基于 `Vue 3 + TypeScript + Vite` 的个人主页项目。

## 页面效果

- 主视觉：毛玻璃卡片风格
- 中央标题：`graphical` 大字，玻璃质感叠加渐变彩色
- 背景：使用 `public/img/wallpaper.jpeg` 作为壁纸
- 字体（英文主字）：`public/font/Rainbow-Party-2.ttf`
- 字体（中文优先）：`public/font/AaPianPianNiShiWoDeQiXu-2.ttf`
- 右下角：作者信息与 GitHub 图标链接（`sobigrice`）

## 本地开发

```bash
npm install
npm run dev
```

默认开发地址一般为 `http://localhost:5173/`。

## 构建与预览

```bash
npm run build
npm run preview
```

## 关键文件

- 页面结构与样式：`src/App.vue`
- 全局样式与字体声明：`src/style.css`
- 入口文件：`src/main.ts`

## 可配置项

- 顶部欢迎文案：`src/App.vue` 中 `.domain`
- 网站简介文案：`src/App.vue` 中 `.tagline`
- 作者名与 GitHub 链接：`src/App.vue` 中 `.author`
