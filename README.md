# CheckpointTree
Mysql， zookeeper, redis等Checkpoint技术研究


<pre>
Checkpoint：
           如果重做日志可以无限地增大，同时缓冲池也足够大，那么是不需要将缓冲池中页的新版本
      刷新回磁盘。因为发生宕机时，完全可以通过重做日志来恢复整个数据库系统中的数据到宕机时
      发生的时刻。
</pre>