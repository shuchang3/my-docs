# my-docs

# My Docs — 个人技术文档网站

![MkDocs](https://img.shields.io/badge/MkDocs-Documentation-blue)
![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Deployed-brightgreen)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-Auto%20Deploy-blue)

## 一、项目简介

本项目是《开源软件技术与实践》课程的第二次实践作业，使用 **MkDocs + Material for MkDocs** 搭建个人技术文档网站，并通过 **GitHub Actions** 自动构建和部署到 **GitHub Pages**。

通过本次实践，我学习了 Markdown 文档编写、静态网站生成、Git 版本控制以及 GitHub Actions 自动化部署的基本方法。

网站主要用于展示个人学习内容、记录技术实践过程，并提供技术文档示例。

## 二、项目地址

* **在线网站：** https://shuchang3.github.io/my-docs/
* **GitHub 仓库：** https://github.com/shuchang3/my-docs/
* **实验报告：** [查看完整实验报告](report/README.md)

## 三、网站内容

网站包含四个主要页面：

| 页面     | 对应文件            | 内容介绍              |
| ------ | --------------- | ----------------- |
| 首页     | `docs/index.md` | 个人介绍及网站内容概览       |
| 关于本项目  | `docs/about.md` | 项目背景、目标和使用技术      |
| 使用指南   | `docs/guide.md` | MkDocs 安装、配置和使用方法 |
| API 参考 | `docs/api.md`   | API 文档格式及示例       |

## 四、技术栈

本项目主要使用以下技术：

* **Markdown**：编写技术文档。
* **Python**：提供 MkDocs 运行环境。
* **MkDocs**：将 Markdown 转换为静态网站。
* **Material for MkDocs**：提供网站主题和导航功能。
* **Git / GitHub**：管理项目源码和版本历史。
* **GitHub Actions**：自动完成网站构建与部署。
* **GitHub Pages**：托管并发布静态网站。

## 五、本地安装与预览

### 1. 克隆项目

```bash
git clone https://github.com/shuchang3/my-docs.git
cd my-docs
```

### 2. 安装依赖

确保已安装 Python，然后执行：

```bash
python -m pip install -r requirements.txt
```

### 3. 启动本地预览

```bash
python -m mkdocs serve
```

在浏览器中访问：

http://127.0.0.1:8000/

即可查看本地网站。

修改 `docs/` 文件夹中的 Markdown 文件并保存后，MkDocs 通常会自动更新预览页面。

### 4. 本地构建

执行：

```bash
python -m mkdocs build --strict
```

MkDocs 会将生成的静态网站文件保存到 `site/` 目录。

## 六、自动部署说明

本项目通过 GitHub Actions 实现自动部署。

当网站文档或相关配置文件的修改被推送到 `main` 分支后，工作流会自动执行以下操作：

1. 检出 GitHub 仓库代码。
2. 配置 Python 环境并安装项目依赖。
3. 使用 MkDocs 构建静态网站。
4. 上传生成的网站文件。
5. 将网站部署到 GitHub Pages。

部署完成后，可以通过以下地址访问网站：

https://shuchang3.github.io/my-docs/

本项目已进行了首次部署以及修改文档后的第二次自动部署验证。

## 七、实验报告

本次实验的详细过程、关键操作截图、遇到的问题、解决方法以及原理分析，均记录在实验报告中。

**点击查看：**

[📄 实践项目 2：个人实验报告](report/README.md)

报告主要包括：

* 实验基本信息
* GitHub 仓库创建
* MkDocs 项目结构与配置
* 本地构建和预览
* GitHub Pages 设置
* GitHub Actions 自动部署
* 第二次推送与自动更新验证
* 问题分析与解决
* 实验原理及实践总结

## 八、实践总结

通过本次实验，我掌握了使用 MkDocs 创建个人文档网站的基本流程，并了解了 GitHub Pages 与 GitHub Actions 的协作方式。

本次实践使我认识到自动化工具在软件开发中的重要作用。相比手动上传网页文件，自动部署能够简化网站维护流程，提高文档更新效率。

今后我会继续利用 Markdown 和 GitHub 记录学习笔记与项目实践，进一步提高文档编写和项目管理能力。

---

**作者：** [shuchang3](https://github.com/shuchang3)
**课程：** 开源软件技术与实践
**项目：** 实践项目 2 — GitHub Pages 自动部署
