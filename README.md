# 山岚古境 · Jade Courtyard

可交互的 Three.js 体素中国古典建筑群：六座古建、对称庭院、飞檐斗拱、水池石桥与秋色园林。

预期访问地址（需先启用 GitHub Pages 并完成部署）：https://Westsea3600.github.io/jade-courtyard/

本仓库为私有仓库；若启用 Pages，发布出的网页可公开访问。私有仓库的 Pages 可用性取决于 GitHub 账户套餐。

打开即显示完整场景，支持拖拽旋转、滚轮缩放、建筑聚焦、自动环游、俯瞰，以及晨曦／暖阳／暮色光照。无需后端。

## 仓库内容

- `index.html`：内联 Three.js、场景代码及样式的独立成品，可直接通过 GitHub Pages 访问或下载离线观看。
- `jade-courtyard-source.zip`：完整可编辑项目，包含 `src/`、Vite 配置、依赖锁文件、离线构建脚本、README 和验收记录；未包含 node_modules。
- `THREE-LICENSE.txt`：Three.js 的 MIT 许可证。
- `.nojekyll`：直接发布静态文件。

## 本地开发

下载并解压 `jade-courtyard-source.zip`，在解压目录执行（建议 Node.js 22.12 或更新版本）：

```sh
npm install
npm run dev
```

构建：

```sh
npm run build
```

将生成的 `dist/山岚古境.html` 复制为本仓库的 `index.html`，提交后 Pages 会自动更新。

本项目采用代码生成几何体，无外部贴图、模型或字体请求。需要支持 WebGL 2 的现代浏览器。
