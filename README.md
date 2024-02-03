# yituliu-docker

一图流 Docker 镜像

## 环境准备

### 安装 Docker 和 Docker Compose

#### Linux

请参考 [Docker CE](https://docs.docker.com/engine/install/) 安装教程。

#### macOS

可以使用 [Docker Desktop](https://docs.docker.com/desktop/install/mac-install/)，或者使用 [Colima](https://github.com/abiosoft/colima) 运行时（推荐）。

```bash
$ brew install colima docker docker-compose
$ mkdir -p ~/.docker/cli-plugins
$ ln -sfn $(brew --prefix docker-compose)/bin/docker-compose ~/.docker/cli-plugins/docker-compose
$ colima start --memory 4 --network-address
```

#### Windows

请参考 [Docker Desktop](https://docs.docker.com/desktop/install/windows-install/) 安装教程。

## 一键运行

```bash
$ docker compose build
$ docker compose up
```

项目启动后，访问 `http://localhost:3000` 即可查看效果。

## TODO

- [ ] 增加可配置项
