# Шаблон при создании проекта Django.

project/\
├── core/\
│   ├── __init__.py\
│   ├── asgi.py\
│   ├── settings.py\
│   ├── urls.py\
│   └── wsgi.py\
└── manage.py

## установка
Создаем дерикторию для витруальнной среды и проекта (в нашем случае будет _"django_code"_)
```commandline
mkdir django_code
```
переходим в созданную дерикторию (в нашем случае будет _"django_code"_)
 ```commandline
 cd django_code
 ```
установка виртуальнйо среды
 ```commandline
 python3 -m venv .venv
```
активация виртуальнной среды 
```commandline
 source .venv/bin/activate
```
> для  деактивация витруальной среды (_если необходимо использовать_) `deactivate`

обновление пакетного менеджера pip 
```commandline
pip install --upgrade pip
```
проверка pip - смотрим версию 
```commandline
pip -V 
```
установка пакета библиотеки Django
```commandline
pip install Django
```
Вы можете проверить, что установка выполнена успешно, введя следующую команду: 
```commandline
django-admin --version
```

установка проекта Django с названием _"project"_ на основе нашего шаблона
```commandline
django-admin startproject --template=https://github.com/DmitrySmor/django_template/archive/main.zip project
```
***
все команды в одну операцию выполняемые друг за другом
```commandline
mkdir django_code && \
cd django_code && \
python3 -m venv .venv &&  \
source .venv/bin/activate && \
pip install --upgrade pip && \
pip install Django && \
django-admin startproject --template=https://github.com/DmitrySmor/django_template/archive/main.zip project && \
cd project
```