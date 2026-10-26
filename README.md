# Nature Portfolio | WiseRobot Studio

中文使用指南：Fork 本仓库，进入 Settings → Pages，Source 选择 GitHub Actions。使用 GitHub 网页直接修改 `content/*.md`，提交后自动发布。

这是演示版，人物、论文、项目内容均为虚构示例。

## 页面功能

首页 / 研究方向 / 论文 / 项目 / 经历 / 联系方式，导航可点击切换页面（Hash 路由，兼容 GitHub Pages 子路径）。支持 Markdown 编辑、PDF 和外部链接、论文筛选、项目分类、主题视觉、响应式布局。

## 内容文件

- `content/profile.md`：姓名、简介、链接、封面照片
- `content/research.md`：研究方向
- `content/publications.md`：论文
- `content/projects.md`：项目、图片
- `content/experience.md`：经历
- `content/contact.md`：联系信息

将照片和公开 PDF 放入 `assets/`，通过相对路径引用。主页会实时读取仓库中最新部署的 Markdown。

**WiseRobot Studio · Nature Portfolio**