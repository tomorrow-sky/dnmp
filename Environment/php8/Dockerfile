FROM ixmo/mine-admin:latest

# 设置时区

ENV TZ=Asia/Shanghai
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

# 切换composer镜像源
RUN composer config -g repo.packagist composer https://mirrors.aliyun.com/composer/

working_dir: "/opt/www"
