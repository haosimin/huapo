# GitHub Pages 部署检查清单

## ✅ 部署前检查

### 1. 文件结构
- [x] `index.html` - 主页面文件
- [x] `styles.css` - 样式文件
- [x] `script.js` - 脚本文件
- [x] `images/` - 图片资源文件夹（包含16张图片，注意：必须使用英文文件夹名）
- [x] `README.md` - 项目说明文档
- [x] `.gitignore` - Git忽略文件

### 2. 路径检查
- [x] 所有图片路径使用相对路径：`images/文件名.png`（必须使用英文文件夹名）
- [x] CSS文件使用相对路径：`styles.css`
- [x] JS文件使用相对路径：`script.js`
- [x] 所有路径都是小写或中文，无特殊字符问题

### 3. 代码质量
- [x] HTML语法正确，无错误
- [x] CSS语法正确，无错误
- [x] JavaScript语法正确，无错误
- [x] 所有图片注释已居中显示

### 4. 图片资源
- [x] 龙岗区地图.png (1.1MB)
- [x] 龙岗高程.png
- [x] 坡度.png
- [x] 龙岗地形起伏等级.png
- [x] 岩组.png
- [x] 断裂.png
- [x] 水系.png
- [x] 植被覆盖.png
- [x] 龙岗路网.png
- [x] 地铁核密度分析.png
- [x] 龙岗公交.png
- [x] 降雨量.png
- [x] 敏感性分析图.png
- [x] 网络分析区域可达性.png
- [x] 网络分析龙岗路网.png
- [x] 风险等级.png

## 🚀 部署步骤

### 步骤 1: 创建 GitHub 仓库
1. 登录 GitHub
2. 点击右上角 "+" → "New repository"
3. 仓库名称建议：`longgang-landslide-analysis` 或 `landslide-detection`
4. 选择 Public（公开）或 Private（私有）
5. **不要**勾选 "Initialize this repository with a README"
6. 点击 "Create repository"

### 步骤 2: 重命名图片文件夹（重要！）
**⚠️ 在上传前必须先重命名文件夹：**
1. 将文件夹 `图` 重命名为 `images`
2. 这是必须的，因为 GitHub Pages 对中文文件夹路径支持不稳定

### 步骤 3: 上传文件
**方法A: 使用 GitHub 网页界面**
1. 在仓库页面点击 "uploading an existing file"
2. 将所有文件拖拽上传（包括重命名后的 `images` 文件夹）
3. 在底部填写提交信息："Initial commit: 龙岗区滑坡检测项目"
4. 点击 "Commit changes"

**方法B: 使用 Git 命令行**
```bash
# 在项目文件夹中执行
git init
git add .
git commit -m "Initial commit: 龙岗区滑坡检测项目"
git branch -M main
git remote add origin https://github.com/你的用户名/仓库名.git
git push -u origin main
```

### 步骤 4: 启用 GitHub Pages
1. 进入仓库的 Settings（设置）
2. 在左侧菜单找到 "Pages"
3. 在 "Source" 部分：
   - Branch: 选择 `main`（或 `master`）
   - Folder: 选择 `/ (root)`
4. 点击 "Save"
5. 等待1-2分钟，GitHub 会显示你的网站地址：
   `https://[你的用户名].github.io/[仓库名]/`

### 步骤 5: 访问网站
- 网站地址会在 Settings → Pages 页面显示
- 首次部署可能需要几分钟时间
- 如果看到 404，等待几分钟后刷新

## ⚠️ 注意事项

1. **文件大小**: 图片文件较大（特别是龙岗区地图.png 1.1MB），首次加载可能需要时间
2. **中文支持**: GitHub Pages 完全支持中文文件名和路径
3. **HTTPS**: GitHub Pages 自动提供 HTTPS 加密
4. **更新内容**: 每次更新文件后，GitHub Pages 会自动重新部署（通常1-2分钟）

## 🔧 常见问题

### 问题1: 图片不显示
- **最重要：检查文件夹名是否为 `images`（不是 `图`）**
- 检查图片路径是否正确（相对路径 `images/文件名.png`）
- 确认图片文件已上传到 GitHub 的 `images` 文件夹
- 检查文件名是否完全匹配（包括大小写）
- 如果文件夹名还是 `图`，需要重命名为 `images` 并重新上传

### 问题2: 样式不生效
- 检查 CSS 文件路径是否正确
- 清除浏览器缓存后重试
- 检查浏览器控制台是否有错误

### 问题3: 网站显示 404
- 确认已启用 GitHub Pages
- 确认 `index.html` 在根目录
- 等待几分钟后重试（首次部署需要时间）

## 📝 更新网站内容

每次更新后：
```bash
git add .
git commit -m "更新内容描述"
git push
```

GitHub Pages 会自动重新部署，通常1-2分钟后更新生效。

