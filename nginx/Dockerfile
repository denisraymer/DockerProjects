FROM ubuntu:latest

# Обновляем пакеты и устанавливаем Nginx
RUN apt-get update && apt-get install -y nginx

# Копируем ваш файл index.html в директорию по умолчанию Nginx
COPY ./html/ /usr/share/nginx/html/

# Копируем файл конфигурации Nginx
COPY ./nginx.conf /etc/nginx/nginx.conf

# Экспонируем порт 80
EXPOSE 80

# Запускаем Nginx в фоновом режиме
CMD ["nginx", "-g", "daemon off;"]
