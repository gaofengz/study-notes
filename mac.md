## Mac远程连接Ubuntu 中文乱码
```
#查看字符集编码设置
locale

#修改设置
vim ~/.zshrc

#文件末尾添加
export LC_ALL=zh_CN.UTF-8  
export LANG=zh_CN.UTF-8

#配置生效
source ~/.zshrc
```
