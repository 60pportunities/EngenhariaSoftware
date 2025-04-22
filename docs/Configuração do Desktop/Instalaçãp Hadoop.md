## Hadoop v.3.4.1

/usr/libexec/java_home -V

> brew install hadoop

> hadoop version

  

```

Hadoop 3.4.1

Source code repository https://github.com/apache/hadoop.git -r 4d7825309348956336b8f06a08322b78422849b1

Compiled by mthakur on 2024-10-09T14:57Z

Compiled on platform linux-x86_64

Compiled with protoc 3.23.4

From source with checksum 7292fe9dba5e2e44e3a9f763fce3e680

This command was run using /opt/homebrew/Cellar/hadoop/3.4.1/libexec/share/hadoop/common/hadoop-common-3.4.1.jar

```

cd /opt/homebrew/Cellar/hadoop/3.4.1/libexec/etc/hadoop/

  

hadoop-env.sh

export JAVA_HOME=/Library/Java/JavaVirtualMachines/temurin-11.jdk/Contents/Home

  
  

core-site.xml

<configuration>

<property>

<name>fs.defaultFS</name>

<value>hdfs://localhost:9000</value>

</property>

</configuration>

  
  

hdfs-site.xml

<configuration>

<property>

<name>dfs.replication</name>

<value>1</value>

</property>

</configuration>

  

mapred-site.xml

  

<configuration>

<property>

<name>mapreduce.framework.name</name>

<value>yarn</value>

</property>

<property>

<name>mapreduce.application.classpath</name>

<value>$HADOOP_MAPRED_HOME/share/hadoop/mapreduce/*:$HADOOP_MAPRED_HOME/share/hadoop/mapreduce/lib/*</value>

</property>

</configuration>

  

yarn-site.xml

  

<configuration>

<property>

<name>yarn.nodemanager.aux-services</name>

<value>mapreduce_shuffle</value>

</property>

<property>

<name>yarn.nodemanager.env-whitelist</name>

<value>JAVA_HOME,HADOOP_COMMON_HOME,HADOOP_HDFS_HOME,HADOOP_CONF_DIR,CLASSPATH_PREPEND_DISTCACHE,HADOOP_YARN_HOME,HADOOP_MAPRED_HOME</value>

</property>

</configuration>

  
  

> hadoop namenode -format

> start-all.sh

> stop-all.sh

> http://localhost:9870

>

> https://didatica.tech/dominando-hadoop-do-zero-com-exemplos-praticos/

>