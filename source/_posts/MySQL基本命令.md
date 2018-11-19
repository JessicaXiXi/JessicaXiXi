#### 基本命令

##### 启动

启动服务： net start mysql

停止服服： net stop 数据库名称

退出：      mysql> quit/exit

---

##### 登录

mysql -u root -p 

admin初始密码为空，故直接回车即可

查询、设置（修改）root用户密码后续待补充

登录mysql：

1、mysql -h 主机IP -P端口号 -uroot -p密码

2、mysql -u root -p

---

##### 操作库

查看数据库中服务器中有哪些库： show databases;

创建一个库： create database 库名;

库已创建后不能重命名

删除一个库：drop database 库名;

---

##### 创建表

创建表：

create table 表名 (

字段名1 类型，

字段名2 类型，

字段名n 类型，

)charset utf8；

------

主键：primary key

自增：auto_increment

不为空：not null

外键：foreign key

foreign key(外键字段名) references mytab2(主键字段名);

---

##### 修改密码

mysql> update mysql.user set authentication_string=password("123456") where user="root";