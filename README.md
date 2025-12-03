# 🚀 超炫酷个人引导页

一个现代化、高性能的个人引导页，支持自定义背景、双引擎搜索、图标网格布局，带有超炫酷的动画效果。

## ✨ 特性

- 🎨 **自定义背景** - 支持图片/渐变背景，可调节亮度、模糊度
- 🔍 **双引擎搜索** - 支持 Google 和百度搜索一键切换
- 🎯 **图标网格布局** - 响应式图标卡片，自适应多端
- ✨ **超炫酷动画**
  - 3D 卡片倾斜效果
  - 鼠标跟随光晕
  - 头像光圈动画
  - 渐变网格背景
  - 点击涟漪效果
  - 滚动淡入动画
- 📱 **完全响应式** - 适配桌面/平板/手机
- ⚡ **高性能优化** - 流畅的 60fps 动画
- 🚀 **一键部署** - 支持 GitHub Pages

## 🎯 快速开始

### 1. 克隆或下载项目

```bash
git clone https://github.com/2200737807/ProfileGenie.git
cd ProfileGenie
```

### 2. 自定义配置

编辑 `config.js` 文件：

```javascript
window.config = {
    profile: {
        avatar: '你的头像URL',
        name: '你的名字',
        bio: '你的个人简介'
    },
    
    background: {
        type: 'image',  // 'image' 或 'gradient'
        image: 'https://your-image-url.com/bg.jpg',
        blur: 0,        // 0-20
        brightness: 0.7 // 0-1
    },
    
    socialLinks: [
        // 你的社交链接
    ],
    
    links: [
        // 你的图标链接
    ]
};
```

### 3. 本地预览

直接用浏览器打开 `index.html` 文件即可预览。

### 4. 部署到 GitHub Pages

1. 创建一个 GitHub 仓库
2. 推送代码到仓库：

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/你的用户名/你的仓库名.git
git push -u origin main
```

3. 在仓库设置中启用 GitHub Pages：
   - 进入 `Settings` → `Pages`
   - Source 选择 `main` 分支
   - 点击 `Save`
   - 访问 `https://你的用户名.github.io/你的仓库名/`

## 🎨 自定义配置说明

### 背景配置

```javascript
background: {
    type: 'image',      // 'image' 或 'gradient'
    image: '图片URL',    // 背景图片
    gradient: '渐变CSS', // 渐变背景
    blur: 0,            // 模糊度 (0-20)
    brightness: 0.7,    // 亮度 (0-1)
    overlay: '遮罩颜色'  // rgba 格式
}
```

### 图标配置

使用 Font Awesome 图标，格式：

```javascript
{
    title: '标题',
    icon: 'fab fa-github',  // Font Awesome 图标类名
    url: 'https://...'
}
```

查找更多图标：[Font Awesome Icons](https://fontawesome.com/icons)

## 🎯 核心动画效果

- **3D 卡片倾斜** - 鼠标悬停时的 3D 透视效果
- **鼠标光晕** - 跟随鼠标的渐变光效
- **头像光圈** - 呼吸式脉动光晕
- **网格背景** - 动态渐变网格动画
- **涟漪效果** - 点击时的水波纹扩散
- **滚动动画** - 元素进入视口时的淡入效果

## 📁 项目结构

```
.
├── index.html      # 主页面
├── style.css       # 样式文件
├── app.js          # 核心逻辑
├── config.js       # 配置文件
└── README.md       # 说明文档
```

## 🌟 推荐背景图片网站

- [Unsplash](https://unsplash.com/) - 高质量免费图片
- [Pexels](https://www.pexels.com/) - 免费素材库
- [Pixabay](https://pixabay.com/) - 免费图片和视频

## 📱 响应式断点

- 桌面：> 768px
- 平板：481px - 768px
- 手机：≤ 480px

## 🚀 性能优化

- CSS 动画使用 GPU 加速
- 使用 `requestAnimationFrame` 优化光晕动画
- Intersection Observer 优化滚动动画
- 最小化重排和重绘

## 📄 许可

MIT License - 自由使用和修改

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！

---

⭐ 如果喜欢这个项目，请给一个 Star！
