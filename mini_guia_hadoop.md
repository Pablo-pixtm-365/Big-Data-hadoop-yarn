
<h1><center>HADOOP</center></h1>

![title](hadoop.jpg)

## Configuration of the four important files

<code>we need to update every xml</code>

### Core-site.xml

***

    
      <configuration>
      <property>
        <name>fs.default.name</name>
        <value>hdfs://localhost:9820</value>
      </property>
      </configuration>
    
    

![title](cap2.jpg)

### mapred-site.xml

****


    <configuration>
      <property>
        <name>mapreduce.framework.name</name>
        <value>yarn</value>
        <description>MapReduce framework name</description>
      </property>
    </configuration>


![tittle](cap3.jpg)

### yarn-site.xml

***

    <configuration>
      <property>
        <name>yarn.nodemanager.aux-services</name>
        <value>mapreduce_shuffle</value>
      </property>
      <property>
        <name>yarn.nodemanager.aux-services.mapreduce.shuffle.class</name>
        <value>org.apache.hadoop.mapred.ShuffleHandler</value>
      </property>

        <!-- Site specific YARN configuration properties -->

    </configuration>


![tittle](cap4.jpg)

### hdfs-site.xml

***

    <configuration>
      <property>
        <name>dfs.replication</name>
        <value>1</value>
      </property>
      <property>
        <name>dfs.namenode.name.dir</name>
        <value>C:\hadoop\data\namenode</value>
      </property>
      <property>
        <name>dfs.datanode.data.dir</name>
        <value>C:\hadoop\data\datanode</value>
      </property>
    </configuration>


![tittle](cap5.jpg)

## Ckeck the that hadoop and java work 

____________________________

<code>hadoop -version</code>

____________________________
    

![title](cap1.jpg)

## Formatting Name node

<code>hdfs namenode -format</code>

![tittle](cap6.jpg)

![tittle](cap8.jpg)

## Starting Hadoop services

<code>start-dfs.cmd</code>

> Two windows wil appear

![tittle](cap9.png)

## Start The Hadoop Yarn Service

<code>start-yarn.cmd</code>

> again two windows will appear

![tittle](cap10.png)

### Check that all services started successfully

<code>jps</code>

***

    14560 DataNode
    4960 ResourceManager
    5936 NameNode
    768 NodeManager
    14636 Jps


### We open the next link

[http://localhost:9870/dfshealth.html](http://localhost:9870/dfshealth.html)

![tittle](cap11.png)

#### Importantan links

> https://www.oracle.com/java/technologies/javase-jdk8-downloads.html#license-lightbox

> https://hadoop.apache.org/old/releases.html

> https://drive.google.com/file/d/1AMqV4F5ybPF4ab4CeK8B3AsjdGtQCdvy/view

> https://hadoop.apache.org/releases.html


```python

```
