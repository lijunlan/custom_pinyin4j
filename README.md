pinyin4j
========

republic from http://sourceforge.net/projects/pinyin4j

optimized by junlan li

mirror
```xml
<mirror>
    <id>junlanli</id>
    <name>junlanli maven</name>
    <url>http://www.junlanli.com:8081/repository/maven-public/</url>
    <mirrorOf>nexus</mirrorOf>
</mirror>
```

### Download ###
Download the jar via maven:
```xml
<dependency>
    <groupId>com.junlanli</groupId>
    <artifactId>pinyin4j</artifactId>
    <version>2.5.1-SNAPSHOT</version>
</dependency>
```


### 多音字识别 ###
在pinyin4j的基础上添加了多音字识别，带近一万个多音词，但是这远远不够，所以用户可设置外挂词库	

### 外挂多音词库 ###
用户配置的外挂词库会覆盖系统中相同词的读音,可用于纠错

配置方式很简单,只需要配置路径即可,相对classpath路径即可
```
MultiPinyinConfig.multiPinyinPath="/yiboliu/my_multi_pinyin.txt"
```

格式同系统的多音词库,如: 
```
吸血鬼日记 (xi1,xue4,gui3,ri4,ji4)
```