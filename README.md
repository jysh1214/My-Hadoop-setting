# My-Hadoop-setting

core-site.xml
```
<property>
    <name>fs.default.name</name>
    <value>hdfs://localhost:9000</value>
</property>
```

yarn-site.xml
```
<property>
    <name>yarn.nodemanager.aux-services</name>
    <value>mapreduce_shuffle</value>
</property>
<property>
    <name>yarn.nodemanager.aux_services.mapreduce.shuffle.class</name>
    <value>org.apache.hadoop.mapred.ShuffleHandler</value>
</property>
```

mapred-site.xml
```
<property>
    <name>mapreduce.framework.name</name>
    <value>yarn</value>
</property>
```

hdfs-site.xml
```
<property>
    <name>dfs.replication</name>
    <value>3</value>
</property>
<property>
    <name>dfs.namenode.name.dir</name>
    <value>file:/home/jyx/hadoop-2.8.5/hadoop_data/hdfs/namenode</value>
</property>
<property>
    <name>dfs.datanode.name.dir</name>
    <value>file:/home/jyx/hadoop-2.8.5/hadoop_data/hdfs/datanode</value>
</property>
```
