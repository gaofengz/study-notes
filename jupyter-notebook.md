## 不挂起后台，一直运行jupyter
```bash
nohup jupyter notebook --no-browser &
```
nohup 命令会忽略所有的挂起信号，确保命令在后台长期执行