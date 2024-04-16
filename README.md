# docker-compose-for-develop
使用docker-compose搭建常用的开发环境，开发时可直接将项目所在的目录挂载到docker，免去本地搭建开发环境的麻烦。
- mongodb
- mysql
- redis
- nginx
- minio
- nodejs
- python


## docker版本
- `docker -v`
  - `Docker version 24.0.5`
- `docker-compose -v`
  - `Docker Compose version v2.23.3`

## 操作
- 启动：在项目根目录执行`sudo docker-compose -f xxx.yaml up -d`。
- 查看容器启动状态：`sudo docker ps -a --filter name=project_comtainer_name`。
- 停止容器：`sudo docker stop project_comtainer_name`。
- 重启容器：`sudo docker restart project_comtainer_name`。
- 删除容器：`sudo docker rm project_comtainer_name`。
- 查看容器日志：`sudo docker logs -f project_comtainer_name`。
- 进入容器：`sudo docker exec -it project_comtainer_name /bin/bash`。
  - 退出:`exit`。
