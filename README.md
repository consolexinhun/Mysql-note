# docker 启动 mysql

```
docker run -d --name mysql -p 13306:3306 -e MYSQL_ROOT_PASSWORD=123qwe mysql

docker exec -it mysql bash

mysql -u root -p

ALTER USER 'root'@'localhost' IDENTIFIED BY '123qwe';

CREATE USER 'test'@'%' IDENTIFIED BY '123qwe';
GRANT ALL PRIVILEGES ON *.* TO 'test'@'%';


```

连接时 allowPublicKeyRetrieval 需要设置为 true，否则连接不上

# MySQL-notes
《MySQL必知必会》笔记

顺序有调整

create.sql和populate.sql为原书给出的sql脚本。

|文件|原书章节|
|---|---|
|1-MySQL基本操作|1-6、19-21章|
|2-数据过滤|7-9章|
|3-数据处理、汇总和分组|10-14章|
|4-联结|15-16章|
|5-组合查询、全文本搜索|17-18章|
|6-其他操作|22-25章|
|7-管理|26-30章|

# SQL 必知必会


