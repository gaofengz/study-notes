## 创建新仓库

选择一个文件夹
```
git init
```
创建一个新的git仓库

## 从远程仓库克隆
```
git clone + address(远程仓库的git地址)
```

## 添加与提交

当你在本地新增加一个文件时，需要将他加入到缓存区
```
git add + <filename>
```

git add

## 提交
```
git commit -m + 描述
```

## 推送
```
git push origin master
```

## 从远程分支next获取更新与本地分支master合并
```
git pull origin next:master
```

## 从远程分支next获取更新与本地当前分支合并
```
git pull origin next
```

## 版本回退
```bash
git log 查看版本提交

git reset --hard ID 使用ID回退到指定版本
```

## 切换分支
```bash
git branch + 分支名
```

111:wq
