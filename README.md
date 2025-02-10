# My docker space

##### Команды

###### 1. Управление образами (Images)

- `docker images` — Показать список всех образов
- `docker pull <image_name>` — Закгрузить образ из Docker Hub (или другого реестра).
- `docker build -t <image_name>:<tag> .` — Создать образ из Dockerfile в текущей директории.
- `docker rmi <image_id>` — Удалить образ.
- `docker tag <image_id> <new_name>:<new_tag>` — Присвоить новый тег образу.
- `docker save -o <filename>.tar <image_name>` — Экспортировать образ в файл.
- `docker load -i <filename>.tar` — Загрузить образ из файла.

###### 2. Управление контейнерами (Containers)

- `docker ps` — Показать список работающих контейнеров.
- `docker ps -a` — Показать список всех контейнеров (включая остановленные).
- `docker run -it --name <container_name> <image_name>` — Запустить контейнер в интерактивном режиме.
- `docker start <container_name>` — Запустить остановленный контейнер.
- `docker stop <container_name>` — Остановить работающий контейнер.
- `docker restart <container_name>` — Перезапустить контейнер.
- `docker rm <container_name>` — Удалить контейнер.
- `docker logs <container_name>` — Посмотреть логи контейнера.
- `docker exec -it <container_name> bash` — Выполнить команду внутри работающего контейнера (например, зайти в bash).
- `docker cp <local_path> <container_name>:<container_path>` — Копировать файл или папку в контейнер.
- `docker cp <container_name>:<container_path> <local_path>` — - Копировать файл или папку из контейнера.

# Компоненты

#### клиент -> служба (daemon) -> хост
