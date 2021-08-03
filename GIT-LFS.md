# GIT LFS 介绍

## 介绍

LFS 是Git 大文件存储（Git Large File Storage）的缩写，Git 使用文本指针来替代大文件（音频、视频、数据集和图片等），将文件存储在远程服务器上。

## 使用步骤

1. 安装 lfs

```shell
git lfs install
```

2. lfs 追踪 pdf 文件

```shell
git lfs track "*.pdf"
```

第一次执行上述命令时会生成 `.gitattributes` 文件，所以还需要将此文件添加到 git 管理中。

```shell
git add .gitattributes
```

3. 提交代码

接下来就正常提交代码即可