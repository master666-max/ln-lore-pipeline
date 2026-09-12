# GitHub 发布补充（仓库绑定信息）

> 本 skill 的官方发布地＝用户 GitHub 私人仓库（详见跨会话记忆 github-repo-ln-lore-pipeline）。
> 发布操作细节（gh 路径/设备码登录/DNS 绕行/curloptResolve）见 references/publish.md 与跨会话记忆。

## 要点速记
1. 仓库：github.com/master666-max/ln-lore-pipeline（PRIVATE，账号 master666-max）
2. staging 本地仓库：迷深工作区 github_ln-lore-pipeline\（main 已推）
3. 更新流程：改 skills 源 → 同步 staging → commit → push（curloptResolve 已全局强制真实 IP）→ gh release create vX.Y
4. 新会话若 gh 未登录：跑设备码登录（_gh_oauth.py 模式，curl --resolve 强制真实 IP）
5. 仓库内容禁止：小说原文、用户真实路径、密钥（发布前跑密钥扫描）
