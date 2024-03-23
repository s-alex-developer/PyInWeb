1. Создать образ:
```bash
docker build . --tag my_img
```

2. Запустить контейнер:
```bash
docker run --name my_cont -d my_img 
```

3. Подключится к контейнеру и проверить новое приветствие:

```bash
docker exec -it my_cont bash -c "curl localhost:80"
```

4. Остановить контейнер:

```bash
docker stop my_cont
```

5. Удалить контейнер:

```bash
docker rm my_cont
```

6. Удалить образ:
```bash
docker rmi my_img 
```