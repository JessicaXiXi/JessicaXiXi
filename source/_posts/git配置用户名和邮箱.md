#### 使用git配置用户名和邮箱

##### 一、在Git目录下创建repository文件夹，打开git-bash，在repository下

创建文件夹并作为仓库，并进入该文件夹

~~~
ls #查看有哪些文件夹
cd repository #进入文件夹
mkdir dirname #创建文件夹
cd dirname
~~~

##### 二、使用git init初始化该仓库，生成.git目录，此为隐藏文件，勾选显示隐藏文件才能看到

~~~
git init #初始化空仓库，生成.git目录，仓库创建完成
~~~

#####三、配置全局用户名/邮箱

~~~
git config --global user.name "username"
git config --global user.email "email"
#配置完成后，通过查看命令看是否配置成功，会写入C盘的.gitconfig文件中
git config --global user.name
git config --global user.email 
~~~

##### 四、配置单个用户名/邮箱

~~~
git config user.name "username"
git config user.email "email"
#查看，配置好的写入当前仓库.git下的config文件
git config user.name
git config user.emai
~~~

