### nexus-docker-compose
nexus私服的docker-compose.yml文件
### 说明
- 仅仅是将[nexus官网安装](https://help.sonatype.com/repomanager3/installation/installation-methods)中的[docker仓库](https://hub.docker.com/r/sonatype/nexus3/)上的命令进行了整合，需提前创建相关`network`和相关`volumes`：
 ```
 #创建network
 docker network create nexus
 #创建volumes
 docker volume create --name=nexus-data
 ```
### 使用
- 安装[docker-compose](https://docs.docker.com/compose/install/)
- 在下载的`docker-compose.yml`目录下运行`docker-compose up -d`启动，运行`docker-compose down`来关闭
