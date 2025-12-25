<img src='https://img.shields.io/badge/Python-3776AB?style=flat-square'><img src='https://img.shields.io/badge/3.13-23283d?style=flat-square'>
<img src='https://img.shields.io/badge/beautifulsoup4-148024?style=flat-square'><img src='https://img.shields.io/badge/4.13-23283d?style=flat-square'>
<img src='https://img.shields.io/badge/requests-0073b7?style=flat-square'><img src='https://img.shields.io/badge/2.32-23283d?style=flat-square'>
<img src='https://img.shields.io/badge/tabulate-ffd343?style=flat-square'><img src='https://img.shields.io/badge/0.9-23283d?style=flat-square'>
<img src='https://img.shields.io/badge/tqdm-cca8c4?style=flat-square'><img src='https://img.shields.io/badge/4.67-23283d?style=flat-square'>

Скрипт авторизации в интерфейсе **phpMyAdmin** и извлечение содержимого таблицы из базы данных.

### Разделы
- [запуск](#запуск)
- [Переменные окружения](#описание-переменных-окружения)

### Запуск

Создать виртуальное окружение
```bash
python3.13 -m venv venv
source venv/bin/activate
```

Установить зависимости
```bash
pip3 install .
```

Добавить переменные окружения в **.env** файл (см. [Переменные окружения](#описание-переменных-окружения))
```bash
cp .env.exapmle .env
```

Запуск
```bash
python3.13 -m src.main --db testDB --table users  # [!] аргументы обязательны
```

#### Описание переменных окружения
| Переменная | Описание                       |
| ---------- | ------------------------------ |
| URL        | Адрес расположения phpMyAdmin. |
| LOGIN      | Имя пользователя.              |
| PASSWORD   | Пароль.                        |
