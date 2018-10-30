## Python虚拟环境 virtualenv 

```
mkdir myproject

cd myproject

virtualenv --no-site-packages venv

# 指定python版本
virtualenv -p /usr/bin/python3 --no-site-packages env

source venv/bin/activate

deactivate #退出当前虚拟环境

# 导出依赖包
pip freeze > requirements.txt
```
