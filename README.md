# SnoreCatcher Website

SnoreCatcher 开发者网站和隐私政策页面。

## 项目结构

```
SnoreCatcherWebsite/
├── index.html          # 主页面（产品介绍）
├── privacy.html        # 隐私政策页面
├── styles.css          # 样式文件
├── README.md           # 项目说明
├── netlify.toml        # Netlify 配置（可选）
└── .gitignore          # Git 忽略文件
```

## 部署到 Netlify

### 方法 1: 通过 Git 连接自动部署

1. 将代码推送到 Git 仓库（GitHub、GitLab 或 Bitbucket）
2. 在 Netlify 控制台连接 Git 仓库
3. 构建设置：
   - **构建命令**: （留空，静态网站无需构建）
   - **发布目录**: `/` 或 `.`
4. 点击 "Deploy site"

### 方法 2: 手动部署

1. 在 Netlify 控制台选择 "Sites"
2. 点击 "Add new site" → "Deploy manually"
3. 将整个文件夹拖拽到部署区域

## 本地预览

可以使用任何静态文件服务器预览网站：

### 使用 Python

```bash
# Python 3
python3 -m http.server 8000

# 然后访问 http://localhost:8000
```

### 使用 Node.js (http-server)

```bash
npx http-server -p 8000
```

### 使用 VS Code Live Server

安装 "Live Server" 扩展，右键点击 `index.html` 选择 "Open with Live Server"

## 自定义配置

### 修改 App Store 链接

在 `index.html` 中搜索并替换：
```html
<a href="https://apps.apple.com/app/snorecatcher" ...>
```

替换为您的实际 App Store 链接。

### 修改样式

编辑 `styles.css` 文件中的 CSS 变量来自定义颜色主题：
```css
:root {
    --primary-color: #2c3e50;
    --secondary-color: #3498db;
    --accent-color: #e74c3c;
    /* ... 其他变量 */
}
```

### 添加开发者联系信息

在 `index.html` 和 `privacy.html` 的 footer 部分，可以添加：
- 邮箱地址
- 社交媒体链接
- 其他联系方式

## 注意事项

1. **App Store 链接**: 请确保在发布前更新 `index.html` 中的 App Store 下载链接
2. **隐私政策**: 根据实际应用功能，可能需要调整 `privacy.html` 中的内容
3. **SEO**: 可以根据需要添加更多 meta 标签和 Open Graph 标签
4. **Analytics**: 如需添加 Google Analytics 或其他分析工具，可以在 `<head>` 部分添加相应代码

## 许可证

版权所有 © 2026 SnoreCatcher
