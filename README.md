# spring_seata_demo
参考"尚硅谷2020最新版SpringCloud(H版&alibaba)框架开发教程全套完整版从入门到精通(大牛讲授spring cloud)"( https://www.bilibili.com/video/BV18E411x7eT?from=search&seid=13634579854688467678)的140-148的内容编写,因为1.3.0的seata差异过大，所以经过两天时间整合了1.3版本，记录下
环境： nacos 1.3.2 + mysql 10.1.34 mariabd + seata 1.3.0
目录结构：
    seata_server：配置文件，下载seata1.3版本以后进行相关配置
    seata-account-service2003：相关项目文件
    seata-order-service2001：相关项目文件
    seata-storage-service2002：相关项目文件
安装 nacos和mysql过程不表，启动nacos，mysql，并执行sql
1.下载seata版本
2.将seata_server内的文件覆盖到seata解压后的文件中
3.执行"sh seata/config/nacos-config.sh  localhost"将seata注册信息注册到nacos
4.执行"seata/bin/seata-server.bat"开启seata服务端
5.导入项目文件到ide中
6.注意下mysql的账号密码与nacos和代码中是否一致
7.启动项目