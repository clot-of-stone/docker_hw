## Task 1

Создать образ

```bash
docker image build . --tag=docker_task1
```

Запустить контейнер

```bash
docker run --name=test1 -d -p 7007:80 docker_task1
```
