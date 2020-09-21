# Git的使用



# 一、**Git的安装[应用]**

最早Git是在Linux上开发的，很长一段时间内，Git也只能在Linux和Unix系统上跑。不过，慢慢地有人把它移植到了Windows上。现在，Git可以在Linux、Unix、Mac和Windows这几大平台上正常运行了。由于开发机大多数情况都是windows，所以本教程只讲解windows下的git的安装及使用。

## （一）**软件下载**

下载地址：<https://git-scm.com/download>

![img](../img-folder/Git/wps258.jpg) 

## （二）**软件安装[应用]**

### 1．**安装git for windows**

 

![img](../img-folder/Git/wps259.jpg) 

一路“下一步”使用默认选项即可。注意：安装路径不要用中文

n 验证安装是否成功

在任何一个目录下右键看是否有菜单

![img](../img-folder/Git/wps260.jpg) 

### 2．**安装TortoiseGit**

下载地址：https://tortoisegit.org/download/

<img src="../img-folder/images/image-30.png" alt="image-20200420180629680" style="zoom: 50%;" />

下载好后执行msi程序进行安装：

![img](../img-folder/Git/wps261.jpg) 

一路“下一步”使用默认选项即可。

默认选项下会启动配置画面：

![img](../img-folder/Git/wps262.jpg) 

由于目前只有英文语言包，默认即可继续下一步。

 

![img](../img-folder/Git/wps263.jpg) 

配置git.exe，已经安装过git-for-windows了所以在此找到git.exe所在的目录。

 

![img](../img-folder/Git/wps264.jpg) 

配置开发者姓名及邮箱，每次提交代码时都会把此信息包含到提交的信息中。

 

![img](../img-folder/Git/wps265.jpg) 

使用默认配置，点击“完成”按钮完成配置。

完整完毕后在系统右键菜单中会出现git的菜单项。

![img](../img-folder/Git/wps266.jpg) 

### 3．**安装中文语言包**

下载地址：https://tortoisegit.org/download/

![image-20200420180822520](../img-folder/images/image-31.png)

安装中文语言包并不是必选项。可以根据个人情况来选择安装。

![img](../img-folder/Git/wps267.jpg) 

直接“下一步”完整完毕。

语言包安装完毕后可以在TortoiseGit的设置中调整语言

![img](../img-folder/Git/wps268.jpg) 

![img](../img-folder/Git/wps269.jpg) 





# 二、**获取课件资料**

1. 使用TortoiseGit：

![img](../img-folder/Git/wps333.jpg) 

2.  填写URL:https://gitee.com/lagouedu/Java_Basics_2020.04.23.git

<img src="../img-folder/images/image-32.png" alt="image-20200420181354691" style="zoom:67%;" />

3. 点击确定：

<img src="../img-folder/images/image-33.png" alt="image-20200420182019892" style="zoom:67%;" />



<img src="../img-folder/images/image-35.png" alt="image-20200420181801331" style="zoom: 80%;" />

<img src="../img-folder/images/image-36.png" alt="image-20200420182053245" style="zoom: 67%;" />

4. 每个模块的课件都在02_课件这个文件夹里，导师会在大家学完本模块后上传下一个模块的课件，并且提醒大家获取，获取方法：

<img src="../img-folder/images/image-34.png" alt="image-20200420182256567" style="zoom: 80%;" />

# 三、上传作业

1. ##### 本地仓库右键TortoiseGit选择设置

<img src="../img-folder/images/image-51.png" alt="image-20200518164545340" style="zoom:80%;" />

2. ##### 选择编辑本地.git/config，输入账号密码，这样避免每次提交的时候输入账号密码

<img src="../img-folder/images/image-52.png" alt="image-20200518164658061" style="zoom:80%;" />

3. ##### 选中要提交的文件——右键，TortoiseGit选择添加

<img src="../img-folder/images/image-45.png" alt="image-20200518150726381" style="zoom:80%;" />



4. ##### 添加完毕后点击提交

<img src="../img-folder/images/image-46.png" alt="image-20200518150749222" style="zoom:80%;" />

5. ##### 填写提交日志信息

<img src="../img-folder/images/image-47.png" alt="image-20200518150842019" style="zoom:80%;" />

6. ##### 提交后选择推送至远程仓库

<img src="../img-folder/images/image-48.png" alt="image-20200518150909850" style="zoom:80%;" />、

7. ##### 默认选择远程仓库的master，默认提交即可

<img src="../img-folder/images/image-49.png" alt="image-20200518150927089" style="zoom: 80%;" />

<img src="../img-folder/images/image-50.png" alt="image-20200518150934728" style="zoom:80%;" />

8. ##### 本地仓库创建规范：

     根目录下12个文件，对应着12个阶段，命名方式如：“第一阶段作业”

     二级目录下对应着模块作业，命名方式如：“第一模块作业”