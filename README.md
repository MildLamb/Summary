# 总结
## Mysql
- mysql 5和mysql 8有所不同
  - driver不同：5 - com.mysql.jdbc.Driver  ， 8 - com.mysql.cj.jdbc.Driver
  - 8 要求url中必须有时区
```yml
spring:
  datasource:
    username: root
    password: *******
    url: jdbc:mysql://localhost:3306/mybatis?useSSL=true&useUnicode=true&characterEncoding=utf-8&serverTimezone=Asia/Shanghai
    driver-class-name: com.mysql.cj.jdbc.Driver
```
## Linux
```bash
开启防火墙：systemctl start firewalld

关闭防火墙：systemctl stop firewalld

查看防火墙状态：systemctl status firewalld
```
- 防火墙添加开放端口命令   firewall-cmd --zone=public --add-port=80/tcp --permanent
- 需要重启防火墙才能看到  重启命令  systemctl restart firewalld.service

## Redis
- 启动客户端：redis-server myconfig/redis.conf
- 启动服务端：redis-cli -p 6379

## SpringCloud
![image](https://user-images.githubusercontent.com/92672384/151465291-cf78316d-4ee6-4122-8b84-4e36296fd1b9.png)

