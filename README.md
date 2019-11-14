# Sharding-JDBC
Sharding-JDBC数据库
这里使用的是hibernate Jpa 
读写分离   分库分表
数据库Mysql
使用的mac操作系统，docker容器安装Mysql，部署在两台机器上，1台作为主数据库，另外一台作为从数据库
localhost:3339  Master 主
localhost:3340  Slave  从
https://www.cnblogs.com/songwenjie/p/9371422.html

https://www.fangzhipeng.com/db/2019/06/26/shardingjdbc-master-slave.html
第一、读写分离  
  主：读写  从：读
第二、分表
  读写分离的好处就是在并发量比较大的情况下，将查询数据库的压力 分担到多个从库中，能够满足高并发的要求
  当数据量比较大的时候，比如单个表的数据量超过了500W的数据，这时可以考虑将数据存储在不同的表中
第三、分库
  在数据量继续扩大，这时可以考虑分库分表，将数据存储在不同数据库的不同表中
