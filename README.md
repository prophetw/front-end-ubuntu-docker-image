[TOC]

# front-end-ubuntu-docker-image


## 安装
```bash

# 下载完 docker 可以配置下载源
## docker -> settings -> Docker Engine 修改配置如下
{
  "registry-mirrors": [
    "https://docker.mirrors.ustc.edu.c",
    "http://hub-mirror.c.163.com",
    "https://registry.docker-cn.com"
  ],
  "insecure-registries": [],
  "debug": false,
  "experimental": true
}
# 打开 cmd/terminal/powershell 拉开发镜像
docker pull prophe89twang/ubuntu-front-end-env:v1
# 启动镜像
docker run -it --name ubuntu-env prophe89twang/ubuntu-front-end-env

```

## 简介
> 关于 docker 开发环境 prophe89twang/ubuntu-front-end-env:v1 简介

> 这个镜像预安装了以下内容

- ubuntu 20.04 系统 默认已经配置到清华下载源
- nodejs 12.20.1
- nvm node 版本管理工具
- npm 需要自行安装 yarn `npm i -g yarn` 即可
- curl
- vim
- zsh 更好用的命令行
- git
- nrm npm/yarn 源管理 默认已经切换到 taobao 镜像源
- setss 会直接走 宿主机 7890 的代理端口 这个可以自行需改
