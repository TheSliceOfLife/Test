- 思而不学  犹豫不决
- 最近我的windows本跑代码快跑废了，搞了一个阿里云学生机，装下anaconda
- 参考： https://blog.csdn.net/ychgyyn/article/details/82258136 

[TOC]

### 1 下载Linux版的Anaconda

下载地址：

- 清华镜像源： https://mirrors.tuna.tsinghua.edu.cn/anaconda/archive/ 
- 官网： https://www.anaconda.com/distribution/ 

我是在清华镜像源下的： Anaconda3-5.3.1-Linux-x86_64.sh

![1585808105368](C:\Users\admin\AppData\Roaming\Typora\typora-user-images\1585808105368.png)

### 2 使用Xftp上传到服务器

- 我在home下新建了个文件夹softwares用于存放软件包

![1585808242856](C:\Users\admin\AppData\Roaming\Typora\typora-user-images\1585808242856.png)

### 3 安装Anaconda 

- 进入softwares：`cd /home/softwares`

  ![1585808446087](C:\Users\admin\AppData\Roaming\Typora\typora-user-images\1585808446087.png)

-  在Linux里面`.sh`文件是可执行的脚本文件，需要用命令bash来进行安装 

- 输入命令： `yum install -y bzip2 `  （ 我安装时缺失环境bzip2，执行了这一句就好了，不一定发生）

- 输入命令：`bash  Anaconda3-5.3.1-Linux-x86_64.sh`

- 安装路径：用户下（我用户root）anconda3

  ![1585808718599](C:\Users\admin\AppData\Roaming\Typora\typora-user-images\1585808718599.png)

-  然后，在安装过程中，我是不断按回车、输入yes默认 

### 4 配置环境变量

-  修改profile文件 ： `sudo vi /etc/profile `

- 在配置文件中添加

  ```
  #Anaconda
  export PATH=$PATH:/位置/anaconda3/bin
  ```

- 我添加的

  ![1585808939022](C:\Users\admin\AppData\Roaming\Typora\typora-user-images\1585808939022.png)

-  最后重新载入配置文件，输入：`source /etc/profile` 

### 5 测试

- 注意要输入python3测试

![1585809249921](C:\Users\admin\AppData\Roaming\Typora\typora-user-images\1585809249921.png)

- 如果输入python，会显示默认的python2版本

![1585809300356](C:\Users\admin\AppData\Roaming\Typora\typora-user-images\1585809300356.png)





```undefined
conda install jupyter jupyterlab
```





|      | 重要 | 次重要 | 不重要 |
| :--: | :--: | :----: | :----: |
|  急  |      |        |        |
| 次急 |      |        |        |
| 不急 |      |        |        |





