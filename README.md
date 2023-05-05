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
1. Создаем дерикторию для витруальнной среды и проекта (в нашем случае будет _"django_code"_)
   ```commandline
   mkdir django_code
   ```
2. переходим в созданную дерикторию (в нашем случае будет _"django_code"_)
    ```commandline
    cd django_code
    ```
3. установка виртуальнйо среды
    ```commandline
    python3 -m venv .venv
   ```
4. активация виртуальнной среды 
   ```commandline
    source .venv/bin/activate
   ```
    > для  деактивация витруальной среды (_если необходимо использовать_) `deactivate`
5. обновление пакетного менеджера pip 
   ```commandline
   pip install --upgrade pip
   ```
6. проверка pip - смотрим версию \
   ```commandline
   pip -V 
   ```
7. установка Django с названием _"project"_ на основе нашего шаблона
   ```commandline
   django-admin startproject --template=https://github.com/DmitrySmor/django_template/archive/main.zip project
   ```
8. Вы можете проверить, что установка выполнена успешно, введя следующую команду: 
   ```commandline
   django-admin --version
   ```
