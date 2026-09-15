# 状态栏发布包

这是 SillyTavern 角色卡《隔壁的青梅竹马变成了长发阴郁少女》的前端状态栏本体。

卡里的 `正则/状态栏界面.html` 会向 `https://testingcf.jsdelivr.net/gh/{GH_USER}/{GH_REPO}/dist/kasumi/界面/状态栏/index.html`
加载本文件。**只要让这个 URL 能访问到，任何导入这张卡的人都能看到状态栏。**

## 你要做的（三分钟）

1. 在 GitHub 新建一个**公开**仓库（任意名字，例如 `st-statusbar`），不要勾选任何初始化（保持空仓库）。
2. 把 `dist/` 这个文件夹推上去（仓库根目录下要有 `dist/`）：
   ```bash
   cd <本项目 deploy 目录>
   git init
   git add dist/
   git commit -m "statusbar"
   git branch -M main
   git remote add origin https://github.com/{你的用户名}/{仓库名}.git
   git push -u origin main
   ```
3. 回来说一声你的「用户名 / 仓库名」，我把卡里 `正则/状态栏界面.html` 的 URL 填好并重新打包。

jsDelivr 会自动从公开仓库根目录的 `dist/` 读取，约十几秒~几小时后生效（第一次最多几分钟）。

> 只推 `dist/` 即可，不必把整个 tavern_helper_template 推上去。