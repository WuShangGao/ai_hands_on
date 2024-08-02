由于 python 自带的源下载速度非常慢，特别是安装一些库的时候，甚至有时会失败。

因此，建议将下载源替换成国内的，下载速度会快很多。总共有两种方法

- 代码替换 （推荐使用这一种）
- 手动替换

## 代码替换

### 设置阿里源(推荐这个)

pip config set global.index-url https://mirrors.aliyun.com/pypi/simple 

pip config set install.trusted-host mirrors.aliyun.com

### 设置清华大学的

pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple/
pip config set install.trusted-host pypi.tuna.tsinghua.edu.cn

## 手动替换

### windows 替换

首先在 windows 当前用户家的目录下，创建一个 pip 文件夹，然后创建一个pip.ini文件，修改文件内容为如下；

[global] 
index-url = http://mirrors.aliyun.com/pypi/simple/ 
[install] 
trusted-host=mirrors.aliyun.com 

1. 记得一定是pip.ini，如果没有开后缀的同学，记得把文件后缀打开，再修改文件的后缀为ini即可。
2. 用户家目录为

C:Users****   # **** 就是当前登录用户名， 比如登录用户名是Luke， 那么就是C:/Users/junxu  

### Mac 替换

会在目录下自动生成，不同系统，目录可能不同，所以使用命令行最靠谱  
~/.config/pip/pip.conf

[global]
index-url = https://mirrors.aliyun.com/pypi/simple

[install]
trusted-host = mirrors.aliyun.com


## 检查

pip config list

## 国内源列表（推荐用阿里云的）

阿里云： [http://mirrors.aliyun.com/pypi/simple/](https://link.segmentfault.com/?enc=Q0Zm%2F%2B6UCn3qb1uBc1rPPQ%3D%3D.doAjYcqDvobYmpMlGj5HAO%2F%2BvVm8II%2FewCdxU%2B5OWmVgyWaP8Ak4Ne3fGK2GWjSa)  
中国科技大学： [https://pypi.mirrors.ustc.edu.cn/simple/](https://link.segmentfault.com/?enc=LxXgri318%2BalmJk7JAAaSA%3D%3D.tMD9XgxajGEvxEHYyJuM07I%2BmZVs%2FfO9D%2BJ7QOj92ATKcQ3V2Xy75LN7ELVN2ftL)  
豆瓣： [http://pypi.douban.com/simple/](https://link.segmentfault.com/?enc=kTI%2FmO2xiIwfSUNcTrmNVA%3D%3D.oCNbhhdTDJmEBLj7RoPCHZSSSXDTkgHCacaBvNLABpw%3D)  
清华大学： [https://pypi.tuna.tsinghua.edu.cn/simple/](https://link.segmentfault.com/?enc=UBsSJmyNBmvKk6qTwKPl5w%3D%3D.sDoJWYrtzjBzLN8Grn5MK3H9v88%2B2MWWTKB7B1DRx%2BOQNj02sekYI25A0E4UCrys)  
中国科学技术大学： [http://pypi.mirrors.ustc.edu.cn/simple/](https://link.segmentfault.com/?enc=v5Jj10ZZuPMeX661X%2BZ8Lw%3D%3D.hY%2FkROt2%2F%2Bzu7N2cqX15ShzzlEuOLWXZfFSIaAr0Hp1gO789VmU7ju2UrYgDfpUc)