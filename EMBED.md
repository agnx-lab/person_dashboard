## 上游嵌入

- 工作方式：整仓魔改（主流）
- 推荐模式：Wrap 原 Workbench UI + 薄 activate + 受管 loopback 同源 API（W2）
- 上游：oyorf/person_dashboard @ person_dashboard-upstream（本目录顶层软链）
- Port 切片：`Workbench/scripts/agnx-local-serve.mjs`；`tools/ensure-workbench-server.mjs` 短跑拉起/复用
- 默认值：Vault=`个人知识库/`；状态落 `apps/data/<appId>/workbench-server.json`；ensure 失败降级 `agnx-miniapp-static` 静态站
