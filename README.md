# 小怡说车拍摄周计划

按小时安排拍前准备、老板出镜、现场拍摄、素材交接与审片发布。电脑端使用，支持周/日视图、任务编辑、拖动改期、调整时长、老板参与筛选、本机保存、撤销、CSV导出和打印。

## 直接使用

[在线打开拍摄周计划](https://zup2885-cell.github.io/xiaoyi-shooting-week-plan/) · [下载完整分享包](https://github.com/zup2885-cell/xiaoyi-shooting-week-plan/archive/refs/heads/main.zip)

下载本仓库的 ZIP，解压后双击 `index.html`。这是包含程序、样式和示例 PDF 的单文件网页，不需要安装 Node.js、申请 API 密钥或登录 ChatGPT。

- `index.html`：可直接打开的完整计划网页。
- `xiaoyi-shooting-plan.pdf`：四页初始示例打印稿。
- `shooting-plan.csv`：可用 Excel 打开的初始计划表。
- `source.zip`：React + Vite 项目源码，供二次开发。
- `THIRD-PARTY-NOTICES.txt`：第三方许可。

修改保存在当前浏览器，不跨设备同步。请导出 CSV 或打印留档；随附 PDF 是初始示例，修改网页后可使用网页内的打印按钮生成新稿。

## 内容说明

以“小怡说车”[已发布视频](https://www.douyin.com/video/7632769091564903410)为样本。公开页核对的发布时间为2026年4月26日10:44，时长5分24秒。

据此补整理2026年4月20日至26日的一周计划，共31项安排，其中13项属于拟定拍摄日、11项需要老板参与。除公开发布点外，具体拍摄日期、钟点、地点和工时均为倒排拟定，须与当事人及原始记录核对。这不是当年已执行的通告单或考勤记录。

## 开发与验证

基于 FullCalendar 6.1.21（MIT）与 React + Vite，按 React Bits Pro Scheduling 6 的公开布局独立制作，没有提取或使用付费 Pro 源码。

解压 `source.zip` 后执行 `npm ci`、`npm run dev`；构建用 `npm run build`，数据检查用 `npm test`。计划内容在 `src/plan.ts`。

已验证PC功能、六项数据检查、四页PDF及1440/1024像素电脑端排版。150个桌面采样帧已全部查看，约3fps VFR；浏览器全部渲染帧验收未完成，不声称严格1:1。没有进行手机端开发或测试。
