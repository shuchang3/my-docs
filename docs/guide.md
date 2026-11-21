
# 使用指南

## 1. 环境准备

在搭建网站之前，需要准备以下工具：

- Git
- Python 3.12
- Visual Studio Code
- GitHub 账号

## 2. 创建项目

首先，在 GitHub 上创建一个公开仓库，然后将仓库克隆到本地电脑。

使用以下命令：

```bash
git clone https://github.com/YOUR-USERNAME/my-docs.git

cd my-docs
```

注意：需要将 YOUR-USERNAME 替换成自己的 GitHub 用户名。

## 3. 安装项目依赖

进入项目目录后，安装 requirements.txt 中的依赖：

```bash
python -m pip install -r requirements.txt
```

## 4. 本地预览网站

执行以下命令：

```bash
python -m mkdocs serve
```

然后打开浏览器，访问：

http://127.0.0.1:8000/

就可以查看网站效果。

## 5. 修改网站内容

在 VS Code 中打开 docs 文件夹，选择需要修改的 Markdown 文件。

例如：

- index.md：修改网站首页。
- about.md：修改项目介绍。
- guide.md：修改使用指南。
- api.md：修改 API 参考。

保存文件后，浏览器中的本地预览页面通常会自动更新。

## 6. 发布网站

完成修改后，使用 Git 提交代码：

```bash
git add .
git commit -m "Update documentation"
git push origin main
```

GitHub Actions 会自动执行构建和部署任务。

## 7. 相关页面

- [返回首页](index.md)
- [关于本项目](about.md)
- [API 参考](api.md)