# MAC安装JDK及环境变量配置

### 一、安装

官网下载 https://www.oracle.com/technetwork/java/javase/downloads/jdk11-downloads-5066655.html

tar包或者dmg，二者区别在于：

tar你自己解压，放在你想要的地方（配置JAVA_HOME的时候是你自己选的位置！）
dmg会把JDK一键安装到 /Library/Java/JavaVirtualMachines下。


安装后 /Library/Java/JavaVirtualMachines目录下文件夹如图：

<img src="../img-folder/JDK/image1.png" alt="img" style="zoom:80%;" />

### 二、环境变量的配置

- 不建议修改/etc/profile，去home文件夹下编辑bash_profile

- 如果没有：touch一个

- 如果看不到：command + shift + .  显示系统隐藏文件

  ```
  vim ~/.bash_profile 
  ```

添加如下内容（注意，第一行是JDK所在目录，这里是我机器的路径，大家写自己的不要照抄）：

```
export JAVA_HOME=/Library/Java/JavaVirtualMachines/jdk-11.jdk/Contents/Home    
export PATH=$JAVA_HOME/bin:$PATH:.   
```

- 以后切换JDK版本，只修改第一行就行了

-  特别注意变量间有分号分隔，结尾是$PATH:.  一般来说PATH变量里会有其他应用的配置，别写乱了

-  如果是JDK8及以前的版本，还需要下面这一句：

  ```
  export CLASSPATH=$JAVA_HOME/lib/tools.jar:$JAVA_HOME/lib/dt.jar:.
  ```

![img](../img-folder/JDK/image2.png)

### 三、 保存修改，并让shell应用新配置

```
source ~/.bash_profile
```

### 四、测试：

```
javac -version

java -version
```

