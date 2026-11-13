# 成都样本 · The Chengdu Sample

一座公园城市的 106 个项目轨迹 —— 单文件交互地图。

## 内容

- **行政区划底图**：成都市域轮廓 + 20 个区县边界，来自 [DataV GeoAtlas](https://datav.aliyun.com/portal/school/atlas/area_selector) `510100_full` / `510100`，已内嵌一份简化轮廓作为离线兜底。
- **水系与路网**：河道、渠道、湖库与高速/快速路/主干道，来自 © OpenStreetMap contributors（ODbL），裁剪至市域并简化。
- **106 个项目**：8 个维度分类、3 条建议路线、中英双语、深色/浅色主题。
- 无外部依赖：样式、脚本、数据、图标全部内联，`index.html` 单文件即可运行。

## 部署（GitHub Pages）

1. 新建仓库（Public）→ 上传本目录下的 `index.html` 与 `.nojekyll`。
2. Settings → Pages → Source 选 **Deploy from a branch** → Branch `main` / `(root)` → Save。
3. 约 1 分钟后访问 `https://<用户名>.github.io/<仓库名>/`。

`.nojekyll` 用于跳过 Jekyll 处理，避免构建环节出问题。

## 说明

- 页面会尝试从 DataV 拉取最新行政区划；取不到时自动使用内置轮廓，断网也能正常查看。
- 地图数据仅用于展示，行政边界以官方发布为准；水系/路网为 OpenStreetMap 快照（2026-11）。
