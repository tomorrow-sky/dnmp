# docker-compose-dnmp

#### 介绍
docker-compose集成环境

[nginx、mysql8、php8、php74、redis 、rabbitmq]


#### 安装教程

1. 下载该docker-compose包

   ```
   git clone https://github.com/tomorrow-sky/dnmp.git
   ```

2. 进入到该目录，执行docker-compose build命令构建

   ```
   cd dnmp
   
   docker-compose build
   ```

3. 启动

   ```
    docker-compose up -d
   ```

4. 查看

   ```
     docker-compose ps
   ```