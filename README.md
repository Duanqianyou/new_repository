# GitHub

## 关键字查询
	1.awesome,去此标签类别中查询项目  python awesome
	2.python tutorial, 查询（python）资料，书籍，文档
	3.socket sample,查询对应技术的代码样本

# GitHUb 三要素

## 1.Repository 仓库
	仓库是github项目管理存储基本单位
	一个仓库中存储一个项目，一个用户可以拥有多个仓库
	一般仓库分为public，private

## 2.Commit 提交
	程序员在整个开发周期，有大量的对代码资源的迭代和修改，
	都可以通过commit的方式进行记录，便于程序员回溯代码，即使这些代码被删除
	
	提交便于使用者观察整个工程的开发流程以及设计流程

## 3.Branch 分支
	在仓库中可以包含多个分支，分支才是代码文件的第
        一存储单位，默认的仓库主分支为master/main
	
        优点：不仅可以管理代码存储，便于多人协作开发



	![1.png](https://i.postimg.cc/4NTZNggK/1.png)
# 仓库内容

	Code，资源存储，代码资源，二进制，项目管理脚本，许可证等等

	issues，使用时遇到的bug 或 进行提交，等待反馈README，使用
	markdown语言编写，工程自述文件，开发进度，版本更新,使用介绍等等

	LICENSE许可证: GPL2.0,3.0.Apahce 2.0，Mit，这
	些许可证，给使用者最大使用权限以及最少的限制

# Git软件，分布式版本控制系统
	仓库管理软件，使用git管理私人代码或企业代码
	![2.png](https://i.postimg.cc/fy1ZQVNy/2.png)

# 设备认证
	1、让网站的账户与设备绑定，后续完成代码的管理，上传下载
	git init // 创建本地仓库  *后续对仓库的操作，都要在仓库位置(master)
	git config -list //查看git的配置文件
	git config --global user.name//用户名
	git config --global user.email//邮箱名
	![3.png](https://i.postimg.cc/d3G7XPbb/3.png)


	SSH生成密文串
	ssh-keygen -t rsa -c "注册邮箱"#创建本地密文 
	*去对应的目录下查找密文文件
	rsa.pub 复制密文，粘贴到 settings -> ssH key and
	GPG -> new ssh key ->粘贴

	ssh -T git@github.com//测试关联是否成功
	2、为目标仓库起别名，定位目标仓库，后续上传
	git remote add orgin(别名)SSH地址(云端仓库地址)
	git remote remove origin#删除地址别名
# 本地设备与云端仓库的交互逻辑
	
	![4.png](https://i.postimg.cc/L89qyWNW/4.png)
	git add code.c #添加内容

	#将缓冲区数据提交到本地仓库
	git commit #提交到本地仓库
	git commit -m "备注信息" //生成提交记录
	git push origin master #将本地仓库内容推到云端仓库
	git status #查看状态
	git rm code.c #删除本地文件及仓库文件
	git restore //恢复被删除（仓库存在）

# 代码更新的依赖关系被破坏
	本地内容要比云端新,完成更新替换， 但是如果直接
  	修改云端内容,导致,本地内容无法再次提交
* 	先拉取 git pul 云端内容 与本地内容合井或操作,而后再次推即可
	
	git pull --rebase origin master
	git rebase --abort#忽略新版，此时还不能上传

	git rebase --skip#需略旧版，更新本地后可以上传

	git rebase --continue #版本合并，解决冲突后可以直接上


# 下载开源代码
	git clone "https仓库地址" #下载开源项目code资源

# 分支Branch
	* 关于分支的相关命令，创建分支、选择分支、合并分支等等
# Markdown 语言
	Markdown,文本修饰语言，用特殊符号修饰正文效果<br>

## 标题修饰符\#

# 标题修饰符（一级标题）
## （二级标题）
### （三级标题）
#### （四级标题）

## 正文内容
        输入正文内容，但是如果需要换行，用\<br\>标签

## 修饰正文
*一段测试文本*
**一段测试文本**
***一段测试文本***
~~一段测试文本~~
测试代码，将`关键字`凸显
## 分割线
用\-\-\-表示分割线
## 引用效果\>表示
> 一级
>> 二级
>>> 三级
>>>> 四级

\-\-\-

## 列表修饰符
### 无序列表\*
* 二次元
  * 原神
    * 启动


### 有序列表 1.
1. 物理学
  1. 粒子
  2. 原子
  3. 铃苣苔

### 混合列表
1. 一级
  * 二级
  2. 三级
  * 四级
### 表格
名称 | 技能 | 排行
-- |:--:| --:|
蝙蝠侠 | 有钱 | 11
祖国人 | 超人 | 1
美国队长 | 五五开 | 2

### 代码片段 ```
```c
        #include<stdio.h>
        int  main(){
        printf("test code\n");
        return 0;

```
```cpp
        #include<iostream>
```


# 超链接
	[抖音](https://www.douyin.com/?recommend=1 "点击访问")

# 插入图片
 
	![图片](https://i.postimg.cc/d3G7XPbb/3.png)
	
	
	






