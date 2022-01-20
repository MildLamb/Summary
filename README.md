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
