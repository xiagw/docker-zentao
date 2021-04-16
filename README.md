## download docker-zentao

`git clone https://github.com/xiagw/docker-zentao.git`

## zentaopms
* Zentao is an agile(scrum) project management system/tool, Free Upgrade Forever!​
* Official: https://github.com/easysoft/zentaopms

## initial preparation work
* [install docker](https://docs.docker.com/engine/install/)
* [install docker-composer](https://docs.docker.com/compose/install/)
* `cp env-example .env`
* update `.env`, include timezone(default UTC)/password, etc.

## startup
`docker-compose up -d`

## setup and access
* First run
* Browser http://host_ip:9080/
* If you see default installation interface of ZenTao, it means that the container is running normally.
* Follow the installation and setup database.
* (fill in `mysql` for the "database server host")

## Difference
This version of docker image is built using debian:10-slim, (zentao/Dockerfile)

Unlike the official image, the official image contains the mysql database,

This image does not contain the database, and the database is loaded with a mysql container (for details, please see docker-compose.yml)

Fork at https://github.com/chaiyd/zentao, optimized and modified, thanks! !