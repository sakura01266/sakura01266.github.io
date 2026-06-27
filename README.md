# 个人开发导航面板


## ✨ 功能亮点
1. **双主题持久化**
   浅色/深色模式切换，使用 LocalStorage 永久保存你的主题偏好，刷新页面不重置。
2. **多分类开发资源聚合**
   - GitHub 快速入口
   - 各类浏览器下载（Chromium、Firefox、Librewolf、Brave等）
   - Linux / BSD 全系列系统镜像（Ubuntu、Arch、Kali、FreeBSD、OpenBSD等）
   - IDE、编译、调试开发工具（VSCode、Python、Android Studio、Pycharm等）
3. **Linux 命令速查工具**
   - 运维、Git、Docker、磁盘、权限、扫描常用命令合集
   - 实时关键词搜索过滤
   - 一键复制，复制成功弹窗通知提示
4. **人性化交互**
   - 页面淡入加载动画，滚动标题自动缩放
   - 滚动超过300px出现「回到顶部」悬浮按钮
   - 顶部浏览器下载提示可一键永久关闭，带平滑收起动画
   - 卡片hover上浮+轻微缩放，交互层次感强
   - 完整移动端适配，手机浏览布局紧凑不溢出
5. **极易自定义**
   所有链接、系统、命令统一在 JS 顶部 `config` 对象配置，无需修改页面DOM结构。

## 🚀 部署方式
### 1. 本地直接打开
将代码保存为 `index.html`，双击用任意浏览器打开即可使用。

### 2. GitHub Pages 在线部署
1. 新建仓库，上传 `index.html`
2. 仓库设置 → Pages，选择对应分支开启静态站点
3. 等待生效，获得公开访问链接

### 3. 其他静态平台
Vercel、Netlify、Coding Pages、Nginx、Apache 等全部兼容，仅需上传HTML文件。

## 🛠 自定义修改指南
1. **新增网站链接**
   修改 `config.githubLinks` / `config.tools`，按 `{name: "名称", url: "链接"}` 格式追加
2. **新增Linux命令**
   在 `config.cmds` 数组内添加命令字符串
3. **修改页面配色**
   CSS `:root` 变量统一管理主色、背景、文字、阴影
4. **调整动画速度**
   修改 `--anim-duration` 变量统一控制全部动画时长

## 🌐 浏览器兼容
Chrome / Edge / Chromium / Firefox / Safari / 移动端浏览器

## 📜 开源说明
本项目为自用静态导航，无版权限制，可自由修改、二次分发、自用部署。

## 📌 后续拓展思路
1. 本地存储自定义收藏链接
2. 板块折叠功能
3. 命令收藏夹
4. 配置JSON导入导出
5. 增加国内镜像站、前端CDN、在线工具分类
