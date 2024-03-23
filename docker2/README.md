### Работа с Docker:

1. Создание образа:
```bash
docker build . --tag my_image
```
2. Запуск контейнера:
```bash
docker run --name my_container -d -p 8888:8000 my_image 
```

3. Проверка стартовой страницы Django проекта >>> [http://127.0.0.1:8888](http://127.0.0.1:8888)


4. Остановка контейнера:
```bash
docker stop my_container
```
5. Удаление контейнера:
```bash
docker rm my_container
```
6. Удаление образа:
```bash
docker rmi my_image
```

### Подготовка проекта:

```bash
python -m venv .venv
```

```bash
".venv/Scripts/activate"
```

```bash
pip install django
```

```bash
python.exe -m pip install --upgrade pip
```

```bash
pip freeze > requirements.txt
```

```bash
django-admin startproject docker .
```

```bash
python manage.py migrate
```

```bash
python manage.py runserver
```
