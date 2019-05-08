注：安装 mongodb redis(其他)模块
- 1. docker ps -a 查看php容器的id
- 2. docker exec -it 容器id bash   进入 命令行
- 3. 执行apt -y update && apt install -y libssh-dev  安装必要的包
- 4. 进入/usr/local/bin, 执行pecl install mongodb && docker-php-ext-enable mongodb
- 5. pecl install redis-3.1.0 && docker-php-ext-enable redis

#安装mysql扩展
- 1. docker-php-ext-install pdo_mysql

#查看rabbitmq队列
- ```http://localhost:15672```
- 账号密码默认guest,guest

#docker_php官方文档 https://hub.docker.com/_/php/
