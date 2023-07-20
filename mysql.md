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
CREATE DATABASE 表名
USE 表名
```

```sql
Age tinyint unsigned
Score double(4,1) #整体长度4,小数长度1

```
