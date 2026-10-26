# Scholar Classic｜维思工坊个人学术主页使用指南

**WISEROBOT STUDIO · Academic Template 2601 · Scholar Classic**

无需编程：**Fork 仓库 → 配置 GitHub Pages → 编辑 Markdown → 自动更新网站**。

## 一、四步快速上手

### 01｜Fork 一份自己的学术网站

**操作示意图**

![Fork 操作示意图](https://raw.githubusercontent.com/jade121213/Academic-Template-2601/main/docs/images/01-fork.svg)

1. 登录 [GitHub](https://github.com/)，打开 [维思工坊学术网站仓库](https://github.com/jade121213/Academic-Template-2603)。
2. 点击右上角 **Fork（派生仓库）**。

![实际截图：点击 Fork](https://raw.githubusercontent.com/jade121213/Academic-Template-2601/main/assets/images/1.png)

3. 选择自己的账号，在 **Repository name（仓库名称）** 中填写想要的名称，再点击 **Create fork（创建派生仓库）**。

![实际截图：填写仓库名称并创建 Fork](https://raw.githubusercontent.com/jade121213/Academic-Template-2601/main/assets/images/2.png)

4. 完成后，你就拥有了一份自己的仓库，后续修改只需要在自己的仓库操作。

### 02｜部署并查看个人网站

**操作示意图（GitHub Actions）**

![GitHub Pages 配置示意](https://raw.githubusercontent.com/jade121213/Academic-Template-2601/main/docs/images/02.svg)

![网站访问示意](https://raw.githubusercontent.com/jade121213/Academic-Template-2601/main/docs/images/03.svg)

1. 在 **自己 Fork 后的仓库** 页面点击顶部 **Settings（设置）**，再点击左侧 **Pages**。

![实际截图：进入 Settings 和 Pages](https://raw.githubusercontent.com/jade121213/Academic-Template-2601/main/assets/images/3.png)

2. 在 **Build and deployment（构建与部署）** 中配置网站发布方式。

> **请注意：** 下面的三张截图演示的是 **Deploy from a branch（从分支发布）** 方法；截图中的 `master` 来自其他演示仓库。**当前 Template2601 已包含 GitHub Actions 自动部署文件** `.github/workflows/pages.yml`，所以更推荐你在 **Source** 下拉框中选择 **GitHub Actions**，然后进入 **Actions** 查看 `Deploy GitHub Pages` 是否运行成功。不要机械照搬截图中的 `master` 分支。

如果你改用截图中的分支发布方式，需要从当前仓库的实际默认分支（通常是 `main`）选择 `/(root)` 并保存，且避免同时使用两种 Pages 部署方法。

![实际截图：选择发布分支并点击 Save](https://raw.githubusercontent.com/jade121213/Academic-Template-2601/main/assets/images/5.png)

3. 保存设置后，GitHub 将开始构建发布；可在 **Actions** 页面查看运行状态。

![实际截图：配置保存成功](https://raw.githubusercontent.com/jade121213/Academic-Template-2601/main/assets/images/6.png)

4. 部署成功后，进入 **Settings → Pages**，点击 **Visit site（访问网站）** 或网页链接。

![实际截图：点击网站访问链接](https://raw.githubusercontent.com/jade121213/Academic-Template-2601/main/assets/images/7.png)

网站地址通常为：

`https://你的用户名.github.io/仓库名/`

### 03｜修改个人简介、论文和项目

**操作示意图**

![修改 Markdown 内容示意](https://raw.githubusercontent.com/jade121213/Academic-Template-2601/main/docs/images/04.svg)

在 Fork 后的仓库里打开 `content/` 文件夹，点击需要修改的 Markdown 文件右上角铅笔图标。修改完成后点击 **Commit changes（提交更改）**。

| 想修改的内容 | 对应文件 |
|---|---|
| 姓名、简介、头像、主题 | `content/profile.md` |
| 研究方向 | `content/research.md` |
| 论文、DOI、PDF 下载链接 | `content/publications.md` |
| 项目及展示图片 | `content/projects.md` |
| 邮箱和联系方式 | `content/contact.md` |

例如在 `content/profile.md` 中修改对应字段（**保留文件原本的 `---` 分隔符**）：

```yaml
name: Li Ming
role: PhD Student
theme: classic
photo: assets/images/my-photo.jpg
```

### 04｜上传图片和学术论文 PDF

**操作示意图**

![上传图片与 PDF 示意](https://raw.githubusercontent.com/jade121213/Academic-Template-2601/main/docs/images/05.svg)

1. 打开 `assets/images/`，选择 **Add file → Upload files（添加文件 → 上传文件）**，上传头像和项目图片。
2. 公开分享的论文 PDF 可以放到 `assets/` 文件夹。
3. 在对应 Markdown 中填写文件路径或论文地址：

```md
Image: assets/images/my-project.jpg
PDF: assets/my-paper.pdf
GitHub: https://github.com/用户名/项目名
```

提交更改后，网站会自动重新发布，**不需要修改前端代码**。

## 二、常见问题

**Fork 后打不开网站？** 先检查自己仓库的 **Settings → Pages** 是否启用了发布，再在 **Actions** 查看部署任务。

**更新 Markdown 后网页没变？** 确认已提交修改，等待部署完成再刷新网页；检查图片路径、文件名大小写是否准确。

**需要购买服务器吗？** 使用 GitHub Pages 托管符合平台政策的静态网站，不需要另购传统 Web 服务器。

**可以换颜色吗？** 在 `content/profile.md` 中把 `theme:` 设置为 `classic`、`dark` 或 `nature`。目前主要改变配色。

**隐私提醒：** 公开仓库中的照片、论文与 Markdown 内容可能被所有人访问，请不要上传敏感信息或未经授权公开的资料。

---

**维思工坊 WISEROBOT STUDIO**  
让技术更简单，让研究成果被更多人看见。
