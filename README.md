# LanzouPlus 市场静态目录

本仓库提供 LanzouPlus 的市场总目录和公告历史。客户端从 GitHub 读取这些文件，并在本地缓存。软件源、图标与 README 由各自的上游 GitHub 仓库提供。

- `market.json`：已经合并发布的市场目录，包含仓库链接、展示名称、发布者、简介与版本资料。
- `announcements.json`：当前及历史公告，包含稳定公告 ID、标题、正文、发布时间和更新时间。

投稿验证服务仅处理用户提交与管理员操作。管理员合并市场目录或发布公告后，会将新文件提交到本仓库。普通用户打开市场无需查询投稿服务器。

## 公告格式

`schema` 为 1，`version` 为递增整数，`announcements` 为数组。每项包含 `id`、`title`、`body`、`publishedAt`、`updatedAt`，时间采用 UTC ISO 8601。

## 参考

目录与上游内容分离的组织方式参考 [AstrBot 插件目录](https://github.com/AstrBotDevs/AstrBot_Plugins_Collection)。本仓库不收集安装包，也不存储管理员凭据或投稿检测码实现。