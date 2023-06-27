## Task 2

Запустить контейнер:

1. Заменить при необходимости значение переменных в файле `crud/stocks_products/.env`
2. Собрать образ командой
```bash
docker image build crud/ --tag=docker_task2
```
3. Запустить контейнер командой
```bash
docker run --name=test2 -d -p 7707:7707 docker_task2
```
