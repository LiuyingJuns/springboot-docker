操作步骤：
在当前目录下：/usr/local/docker/springboot-project/docker-compose-springboot
在执行下面的步骤之前，要创建redis和mysql对应的目录，将mysql的my.cnf 和 redis 的redis.conf文件提前准备好，
并在docker-compose.yml 文件中配置好 volumes


1.将jar包放到上面去，重新命名为：docker_boot.jar，参考Dockerfile里面的镜像
2.对Dockefile文件构建镜像，执行以下命令：
    docker build -t springboot_docker:1.0 .   镜像名称参考docker-compose.yml 文件

3.构建镜像完成之后，执行容器编排命令，在当前目录下启动服务，命令如下：
    docker-compose up -d

4.如果要关闭编排，执行命令：docker-compose down
