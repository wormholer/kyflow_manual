#### DATAFLOW安装及配置

##### 快速安装

1. 下载 Dataflow.tar.gz 压缩包

2. 解压

   `tar -zxvf Dataflow.tar.gz /YOUR_DIR`

##### 配置

配置**DATAFLOW**

用户需要指定**DATAFLOW**运行所需的JDBC连接：

 编辑： `vi INSTALL_DIR/conf/dataflow.properties`

 配置jdbc数据库：`jdbcUrl=jdbc:mysql://localhost/DATABASE_NAME`

jdbc数据库的用户名及密码：

`user = root`

`password = 12345`

**KYSCHEDULER** WebUI登陆用户名及密码：

`login.username=admin`

`login.password=admin`

 配置节点角色

dataflow.role=master`

配置日志路径

dataflow.log.path=/tmp/dataflow`

