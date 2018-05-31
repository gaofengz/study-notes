# 使用docker启动django

## 需要先安装docker-compose
```
sudo pip3 install docker-compose
```

### 创建Dockerfile
```
 FROM python:3
 ENV PYTHONUNBUFFERED 1
 RUN mkdir /code
 WORKDIR /code
 ADD requirements.txt /code/
 RUN pip install -r requirements.txt
 ADD . /code/
 ```

 ### 创建requirements.txt
 ```
 Django>1.8,<2.0
 psycopg2
 ```

 ### 创建docker-compose.yml
 ```
 version: '3'

services:
  db:
    image: postgres
  web:
    build: .
    command: python3 manage.py runserver 0.0.0.0:8000
    volumes:
      - .:/code
    ports:
      - "8000:8000"
    depends_on:
      - db
```

### 创建django项目
```
sudo docker-compose run web django-admin.py startproject composeexample .
```