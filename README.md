# Haskell Notebook

个人学习 Haskell 的过程中所整理的一些笔记，采用 Jupyter Notebook 格式书写，绝大部分内容来自《Haskell 趣学指南》。

要在本地运行此文档，你需要安装 [IHaskel](https://github.com/gibiansky/IHaskell) 内核，为了方便，
建议你直接使用 [ihaskell-notebook](https://hub.docker.com/r/crosscompass/ihaskell-notebook) docker 镜像，
此 docker 镜像大约 **1.5G**，请确保你有足够的空间和良好的网络环境。

## 使用指南

1. 拉取 ihaskell-notebook 镜像：`docker pull crosscompass/ihaskell-notebook`
2. 运行 ihaskell-notebook 镜像：`docker run --rm -p 8888:8888 -v $PWD/notebook:/home/jovyan/work --user root --name ihaskell_notebook crosscompass/ihaskell-notebook`
3. 打开终端中输出的网址，进入 Jupyter Notebook 的 `work` 文件夹。

此外，倘若你想使用 Jupyter Lab，请在运行 ihaskell-notebook 镜像时添加参数 `--env JUPYTER_ENABLE_LAB=yes`。
