# Sales English OS v0.2

手机优先的60天海外储能销售英语训练网页应用，包含12篇电话+13篇会议专题、间隔复习和每日课程。

## 通过 GitHub Pages 公开网站

**使用注意：GitHub Pages 网站对外可访问。不要在仓库代码中放客户机密、公司报价、账号密码或 API Key。**

1. 在 GitHub 创建仓库 `sales-english-os`，建议 Public，默认分支 `main`。如准备由 ChatGPT GitHub 连接器上传，请先勾选 Initialize with README 并授权连接器访问新仓库。
2. 上传本目录的文件到仓库根目录（注意 `index.html` 必须在根目录，不要放在 `sales_english_os_github_ready/` 子文件夹内）。
3. 进入 **Settings → Pages → Build and deployment → Source → GitHub Actions**。
4. 进入 **Actions → Publish Sales English OS to GitHub Pages**，如果没有自动部署，点击 **Run workflow**。
5. 在 Settings → Pages 查看真实的 Visit site 地址；如果仓库名为 `sales-english-os` 且用户为 `thinkinspiron-star`，通常是 `https://thinkinspiron-star.github.io/sales-english-os/`，**未完成前不要把该地址当作已经上线**。
6. 用 Android Chrome 打开 HTTPS 网址，菜单里选择 **安装应用** 或 **添加到主屏幕**。

如果不想使用 workflow，也可以删除 `.github/workflows/pages.yml`，设置 Pages 发布源为 Deploy from a branch → main → /(root)，效果相同。

## 功能边界

- 练习记录保存在浏览器本地 `localStorage`；清理站点数据可能丢失，建议定期在应用设置中导出 JSON。
- 朗读依靠设备 TTS，语音识别依赖浏览器/网络，不是实时AI外教，也没有后台云同步。
- 本项目内容为原创英语教学素材，内部的业务与技术模拟不代表公司合同承诺。
- 不包含任何 API Key、数据库账号或后台服务。

版本：v0.2；适用于子路径 GitHub Pages（静态资源使用相对URL）。
