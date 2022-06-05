FROM mysql:8.0

# 设置时区

ENV TZ=Asia/Shanghai
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

#RUN chmod 770 /var/log/mysql/