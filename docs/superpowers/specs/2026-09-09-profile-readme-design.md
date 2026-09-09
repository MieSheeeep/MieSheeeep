# GitHub Profile README 同款改造设计

## 目标

以 `brunotacca/brunotacca` 的 GitHub 个人主页 README 为版式来源，为 `MieSheeeep/MieSheeeep` 制作一份可直接使用、便于继续个性化的版本。

## 采用方案

- 保留原版的整体信息层次：顶部介绍、联系方式、主技术栈、学习中的技术、GitHub 统计和访问计数。
- 所有依赖 GitHub 用户名的动态图片统一改为 `MieSheeeep`。
- 不保留原作者的姓名、邮箱、公司、家庭情况、LinkedIn 和赞助链接。
- 暂时未知的个人资料使用明显的 `【请修改：...】` 文本，避免误把原作者经历发布到用户主页。
- 保留 shields.io 技术徽章，作为后续删改的现成素材。
- 去掉英语、法语、葡萄牙语切换，因为当前仓库只有一个 README。
- 顶部使用 Markdown 标题代替原作者专属 SVG，避免显示错误姓名；后续可另做个人横幅。
- 在 README 源码中增加中文注释，标明各个可修改区域；注释不会显示在 GitHub 页面中。

## 文件范围

- 修改根目录 `README.md`。
- 不引入构建脚本或运行时依赖。
- 不复制原作者专属图片资源。

## 验收标准

- README 中不存在 `brunotacca`、原作者邮箱、公司、LinkedIn 或 Ko-fi 信息。
- GitHub 统计、语言统计、连续提交和访问计数均指向 `MieSheeeep`。
- Markdown/HTML 标签结构完整。
- 用户能通过搜索 `请修改` 快速找到所有需要个性化的位置。

## 验证方式

- 搜索原作者标识，确认无遗留。
- 搜索 `MieSheeeep`，确认动态服务参数已替换。
- 检查 HTML 标签和 `<details>` 区块是否成对闭合。
