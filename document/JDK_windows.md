## 								**JDK11 下载与安装** 

### 相关的概念

​	JDK - 称为Java开发工具包（ Java Development Kit）。Java开发人士需 要下载和安装JDK，目前的主流版本为JDK11。 

​	JRE - 称之为Java SE运行时环境（Java SE Runtime Environment），提供了运行Java应用程序所必须的软件环境等。无论是开发还是运行Java应用都必须安装。

### JDK11下载

​	步骤1： 访问 https://oracle.com

​    步骤2： 注册，并登陆。 （国内无法正常注册） 

​    步骤3： 跳转到官网下载页面：https://www.oracle.com/java/technologies/javase-jdk11-downloads.html

​    步骤4： 选择对应的版本

<img src="../img-folder/JDK/image-20200415170224264.png" alt="image-20200415170224264" style="zoom:80%;" />

#### JDK11安装

​    步骤1：双击安装包

​      <img src="../img-folder/JDK/image-20200415171214095.png" alt="image-20200415171214095" style="zoom:80%;" />

​	步骤2：看图安装软件

<img src="../img-folder/JDK/image-20200415180411359.png" alt="image-20200415180411359" style="zoom:80%;" />

<img src="../img-folder/JDK/image-20200415180427465.png" alt="image-20200415180427465" style="zoom:80%;" />

<img src="../img-folder/JDK/image-20200415180300739.png" alt="image-20200415180300739" style="zoom:80%;" />

​	步骤3：配置环境变量（这里要区分win10和win7）

​	win10：此电脑——右键属性

​									<img src="../img-folder/JDK/image-20200415172211019.png" alt="image-20200415172211019" style="zoom:80%;" />

<img src="../img-folder/JDK/image-20200415172301882.png" alt="image-20200415172301882" style="zoom:80%;" />

<img src="../img-folder/JDK/image-20200415172320632.png" alt="image-20200415172320632" style="zoom:80%;" />

​								<img src="../img-folder/JDK/image-20200415180701164.png" alt="image-20200415180701164" style="zoom:80%;" />





<img src="../img-folder/JDK/image-20200415180616987.png" alt="image-20200415180616987" style="zoom:80%;" />

安装完毕

win7：计算机 => 右击，选择属性 => 高级系统设置 => 高级 => 环境变量 => 系统变量 => 找到Path，点击编辑 => 将javac.exe所在的路径信息配置到Path变量值的最前面，加上英文版的分号 => 一路点击确定即可

![image-20200415175358653](../img-folder/JDK/image-20200415175358653.png)

<img src="../img-folder/JDK/image-20200415175445784.png" alt="image-20200415175445784" style="zoom:80%;" />

![image-20200415175507782](../img-folder/JDK/image-20200415175507782.png)

![image-20200415175548161](../img-folder/JDK/image-20200415175548161.png)

<img src="../img-folder/JDK/image-20200415175927069.png" alt="image-20200415175927069" style="zoom:80%;" />

### JDK测试安装成功

win+R键弹出运行，输入cmd，点击确定



![image-20200415180809351](../img-folder/JDK/image-20200415180809351.png)



输入java -version命令，如下图则环境配置成功



![image-20200415180852064](../img-folder/JDK/image-20200415180852064.png)



### jdk生成对应的jre文件

一、左下角点击搜索，输入cmd，右键单击，选择以管理员的身份运行cmd。



<img src="../img-folder/Git/temp1.jpg" alt="img" style="zoom:25%;" />

二、输入“CD”+“jdk下载保存的位置”，如下图。

<img src="../img-folder/Git/temp2.jpg" alt="img" style=" width:500px;height:200px;zoom:25%;" />

三、在下一行中输入如下命令即可。
		bin\jlink.exe --module-path jmods --add-modules java.desktop --output jre
<img src="../img-folder/Git/temp3.jpg" style="zoom:80%;" />

检查jdk目录，查看jre是否生成成功