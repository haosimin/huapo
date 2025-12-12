# 龙岗区滑坡检测 - 地质灾害易发性分析

基于ArcGIS的龙岗区滑坡地质灾害易发敏感性分析项目展示网站。

## 项目简介

本研究以深圳市龙岗区为研究对象，基于ArcGIS平台，结合多源地理空间数据，开展滑坡地质灾害易发性评价。通过系统分析高程、坡度、地形起伏度、岩组类型、断裂构造距离、水系距离、植被覆盖、道路网络、公共交通密度及年均降雨量等10项孕灾因子，揭示各因子对滑坡发育的影响机制。

## 技术栈

- HTML5
- CSS3
- JavaScript (原生)

## 文件结构

```
.
├── index.html          # 主页面
├── styles.css          # 样式文件
├── script.js           # 交互脚本
├── README.md          # 项目说明
├── .gitignore         # Git忽略文件
└── 图/                # 图片资源文件夹
    ├── 龙岗区地图.png
    ├── 龙岗高程.png
    ├── 坡度.png
    └── ...
```

## 部署到 GitHub Pages

### 方法一：通过 GitHub 网页界面

1. 在 GitHub 上创建一个新仓库
2. 将所有文件上传到仓库
3. 进入仓库的 Settings（设置）
4. 在左侧菜单找到 Pages（页面）
5. 在 Source（源）部分，选择 `main` 分支（或 `master` 分支）
6. 点击 Save（保存）
7. 等待几分钟，GitHub 会提供一个网址，格式为：`https://[你的用户名].github.io/[仓库名]/`

### 方法二：通过 Git 命令行

```bash
# 初始化 Git 仓库
git init

# 添加所有文件
git add .

# 提交更改
git commit -m "Initial commit: 龙岗区滑坡检测项目"

# 添加远程仓库（替换为你的仓库地址）
git remote add origin https://github.com/你的用户名/仓库名.git

# 推送到 GitHub
git branch -M main
git push -u origin main
```

然后在 GitHub 仓库设置中启用 GitHub Pages（参考方法一）。

## 本地预览

直接在浏览器中打开 `index.html` 文件即可预览。

或者使用本地服务器：

```bash
# 使用 Python
python -m http.server 8000

# 使用 Node.js (需要先安装 http-server)
npx http-server
```

然后在浏览器中访问 `http://localhost:8000`

## 注意事项

- 确保所有图片路径使用相对路径（已使用 `图/` 相对路径）
- GitHub Pages 支持中文文件名和路径
- 图片文件较大，首次加载可能需要一些时间
- 建议使用现代浏览器（Chrome、Firefox、Safari、Edge）

## 作者

郝思敏 魏永琦 郝鑫

人文社科学部 资源与环境

## 许可证

本项目仅用于学术研究展示。

