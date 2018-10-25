## nginx安装
```
sudo apt update
sudo apt install nginx
```

## nginx卸载
```
sudo apt-get remove nginx nginx-common # 卸载删除除了配置文件以外的所有文件。

sudo apt-get purge nginx nginx-common # 卸载所有东东，包括删除配置文件。

sudo apt-get autoremove # 在上面命令结束后执行，主要是卸载删除Nginx的不再被使用的依赖包。

sudo apt-get remove nginx-full nginx-common #卸载删除两个主要的包。
```

## nginx相关操作
```bash
启动
sudo nginx

关闭
sudo nginx -s stop

重启
sudo nginx -s reload
```

## Mac下相关配置
```
#homebrew安装nginx
brew install nginx

#Mac下的配置文件目录
/usr/local/etc/nginx
```

