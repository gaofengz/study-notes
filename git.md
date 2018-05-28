# 创建新仓库
2

3
选择一个文件夹
4
```
5
git init
6
```
7
创建一个新的git仓库
8

9
# 从远程仓库克隆
10
```
11
git clone + address(远程仓库的git地址)
12
```
13

14
# 添加与提交
15

16
当你在本地新增加一个文件时，需要将他加入到缓存区
17
```
18
git add + <filename>
19
```
20

21
git add
22

23
# 提交
24
```
25
git commit -m + 描述
26
```
27

28
# 推送
29
```
30
git push origin master
31
```
32

33
# 从远程分支next获取更新与本地分支master合并
34
```
35
git pull origin next:master
36
```
37

38
# 从远程分支next获取更新与本地当前分支合并
39
```
40
git pull origin next
41
```
