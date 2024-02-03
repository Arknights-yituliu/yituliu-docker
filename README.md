# yituliu-docker

一图流 Docker 镜像

## 环境准备

### 安装 Docker

#### macOS

推荐使用 [Colima](https://github.com/abiosoft/colima) 作为运行时。

```bash
brew install colima docker
colima start --memory 4 --network-address
```

### 安装 Docker Compose

#### macOS

```bash
brew install docker-compose
mkdir -p ~/.docker/cli-plugins
ln -sfn $(brew --prefix docker-compose)/bin/docker-compose ~/.docker/cli-plugins/docker-compose
```

## 一键部署

```bash
docker compose build
docker compose up
```

项目启动后，访问 `http://localhost:3000` 即可查看效果。

## TODO

- [ ] Linux Docker 环境教程
- [ ] Windows Docker 环境教程
- [ ] 增加可配置项
