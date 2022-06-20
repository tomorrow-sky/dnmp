# docker-compose-dnmp

#### 介绍
docker-compose集成环境

[nginx、mysql8、php8、redis、rabbitmq]


#### 安装教程

1. 下载该docker-compose包

   ```
   git clone https://github.com/tomorrow-sky/dnmp.git
   ```

2. 进入到dnmp/Site站点目录，下载MineAdmin项目

   ```
   cd dnmp/Site
   
   git clone https://gitee.com/xmo/MineAdmin.git
   ```

3. 切换到dnmp/Environment目录，执行docker-compose build 构建环境
   ```
   cd ../Environment
   
   docker-compose build
   ```

4. 启动

   ```
    docker-compose up -d
   ```

5. 查看

   ```
     docker-compose ps
   ```

6. 进入php8容器

   ```
     docker-compose exec php8 bash
   ```

7. 进入项目，并安装composer依赖包
   ```
     cd /opt/www/MineAdmin
     
     composer install
   ```

8. 安装项目并启动
   ```
     # 检查环境并生成.env文件
     php bin/hyperf.php mine:install
     
     # 执行数据迁移，生成数据表
     php bin/hyperf.php mine:install
   
     # 启动项目
     php bin/hyperf.php start
   ```