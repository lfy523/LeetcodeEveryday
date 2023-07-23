# MySQL

数据库(DataBase,DB)

～管理系统( ～ manage system)

SQL:操作关系型数据库编程语言

关系型数据库（RDBMS）：建立在关系模型基础上，由多张相互连接的二维表组成的数据库（通过表）

一个数据库可创建多张表，可创建多个数据库



SQL

通用语法

* ；结尾
* 空格／缩进
* 不区分大小写
* 注释：#

分类

* DDL：定义语句
* DML：操作语句(manipulate)
* DQL：查询语句（query）
* DCL：控制语句

DDL

```sql
 SHOW TABLES #查询所有表
 DESC 表名#查询表结构
 CREATE TABLES 表名
```

varchar  字符串

```sql
CREATE DATABASE 数据库名
USE 数据库名
```

```sql
Age tinyint unsigned
Score double(4,1) #整体长度4,小数长度1
#一般不直接存二进制
char(10) #定长，性能高
varchar(10) #变长，性能低
Username varchar
age char(1)


```

表操作＿修改

```sql
ALTER TABLE 表名 ADD 字段名 类型（长度）［COMMENT 注释］［约束］
ALTER TABLE 表名 MODIFY 字段名 新类型 #只能改数据类型
ALTER TABLE 表名 CHANGE 旧名 新名 新类型
```

删除

```sql
ALTER TABLE 表名 DROP 字段名
```

修改表名

```sql
ALTER TABLE 表名 RENAME TO 新表名
```

删除表

```sql
DROP TABLES IF EXISTS 表名
TRUNCATE TABLE 表名#删除并新建，但数据会消失
```

MySQL 图形化

Datagrip



DML:对表中数据进行增删改

```sql
添加(INSERT)
修改(UPDATE)
删除(DELETE)
```

```sql
INSERT INTO 表名 （字段名1,字段名2) VALUES (值1, 值2)#指定字段
INSERT INTO 表名 VALUES (值1,值2) #给全部字段
INSERT INTO 表名 （字段名1, 字段名2) VALUES (值1, 值2),(值1, 值2),...
INSERT INTO 表名 VALUES (值1, 值2),(值1, 值2),... #批量添加
```

注意事项:日期，字符串应包含在引号内

```sql
UPDATE 表名 SET 字段名1=值1, 字段名2 =值2, …[WHERE 条件]; 
UPDATE emp SET name = 小昭, gender =女 where Id= 1;
```

```sql
DELETE FROM 表名 [WHERE 条件]
```
