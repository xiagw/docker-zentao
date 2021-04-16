## 下载 docker-zentao

`git clone https://github.com/xiagw/docker-zentao.git`

## 禅道
* 禅道是专业的研发项目管理软件
* 官网：https://github.com/easysoft/zentaopms

## 准备
* [install docker](https://docs.docker.com/engine/install/)
* [install docker-composer](https://docs.docker.com/compose/install/)
* `cp env-example .env`
* 修改.env文件内部参数/时区(默认UTC)/密码等信息

## 启动
`docker-compose up -d`

## 访问和安装
* 首次运行
* 浏览器访问http://ip:9080
* 如果网页界面显示禅道默认安装界面，说明容器运行正常。
* 依照禅道安装程序（数据库服务器主机填写`mysql`）安装成功，就可以使用了。

## 差异说明
此版本 docker image 使用debian:10-slim 构建，(zentao/Dockerfile)

与官方 image 不同，官方 image 包含mysql数据库，

此镜像不包含数据库，数据库额外加载mysql容器，(详细请查看 docker-compose.yml)

fork 于 https://github.com/chaiyd/zentao，做了优化和修改，感谢！！
