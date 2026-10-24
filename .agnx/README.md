# 个人知识工作台 胶水说明

- `dist/index.js` — 子应用入口（打包产物，必须入库）
- `manifest.json` / `config.json` — 身份与上游出处（`oyorf/person_dashboard`）

本子应用只嵌入上游的静态页面，不含上游源码副本；需要重建时：

```bash
git clone --filter=blob:none https://github.com/oyorf/person_dashboard.git
npm run build
```
