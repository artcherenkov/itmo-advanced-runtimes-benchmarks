FROM denoland/deno:latest

WORKDIR /app

# Копирование файла сервера
COPY ./index.js .

# Настройка прав доступа для Deno
RUN chmod 755 index.js

# Открываем порт
EXPOSE 3102

# Запуск сервера с разрешениями для сети и переменных окружения
CMD ["deno", "run", "--allow-net", "--allow-env", "index.js"] 