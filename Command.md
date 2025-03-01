# Команды

## Pip

- pip install package-name - Установка пакета
- 'pip install package-name==4.8.2' - Установка пакета версии 4.8.2
- python3.13.1 -m pip install package-name - Установка пакета для Python v3.13.1
- pip uninstall packege-name - Удаление пакета
- python -m pip install --upgrade pip - Обновление pip
- pip list - Вывод списка установленных пакетов
- pip freeze > requirements.txt - Запись установленных библиотек в файл
- pip install -r requirements.txt - Установка зависимостей сохраненых в проекте

## Poetry

- poetry init - Инициализировать пакет в существующем проекте

Активация виртуального окружения:
- poetry shell - Активировать виртуальное окружение (Poetry 1.8.5) в Poetry 2.0.0 работает с плагином poetry-plugin-shell
- poetry env activate или .\.venv\Scripts\activate - Активировать виртуальное окружение (Poetry 2.0.0)
- pip install poetry-plugin-shell - Команда для установки плагина poetry-plugin-shell

- poetry add requests - Установка библиотек, зависимостей. В пример указан requests.
- poetry show --tree - Посмотреть дерево зависимостей
- poetry add --group dev requests - Установка группы develop зависимостей. В пример указан requests.

## Poetry add group dev

- poetry add --group dev mypy - Установка Mypy
- poetry add --group dev pytest - Установка Pytest
- poetry add --group dev pytest-cov - Установка Pytest-cov
  poetry run pytest --cov - Запуск тестов с оценкой покрытия
  pytest --cov=src --cov-report=html - Генерация отчета по покрытию в HTML формате

## Poetry add group lint

- poetry add --group lint black - Установка Black
- poetry add --group lint isort - Установка Isort
- poetry add --group lint flake8 - Установка Flake8


## .env

- pip install python-dotenv - установка библиотеки Dotenv для чтения файла .env

## Git

- git init - Создать репозиторий
- git status - Посмотреть статус репозитория
- git add 'Название файла' - Добавить индекс (выбрать файл для коммита)
- git commit -m 'Краткое описание что, было сделано' - Файлы из индекса отправить в репозиторий
- git log - Список всех выполненных коммитов, отсортированных по дате выполнения
- git show 'commit_hash' - Все изменения, сделанные в рамках одного коммита по хешу
