# Используйте официальный образ Python как базовый
FROM python:3.9

# Установите рабочий каталог в контейнере
WORKDIR /usr/src/app

# Установите зависимости
COPY requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt

# Копируйте проект в контейнер
COPY . .

# Укажите порт, на котором будет работать приложение
EXPOSE 8000

# Команда для запуска сервера
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]