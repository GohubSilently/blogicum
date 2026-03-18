# Blogicum - блог на базе фреймвока Django.

[![Python](https://img.shields.io/badge/-Python_3.12-3771a1?style=flat&logo=Python&logoColor=ffffff)](https://www.python.org/)
[![Django](https://img.shields.io/badge/-Django_5.1-092E20?style=flat&logo=django&logoColor=ffffff)](https://www.djangoproject.com/)
[![Bootstrap](https://img.shields.io/badge/-Bootstrap%205-7952B3?style=flat&logo=bootstrap&logoColor=ffffff)](https://getbootstrap.com/)

Ознакомиться можно тут: [Blogicum](https://gohub.pythonanywhere.com)

Автор – [Халин Вадим](https://t.me/gohub1)

---

## Оглавление
- [Описание](#описание)
- [Функционал](#функционал)
- [Основные технологии](#основные-технологии)
- [Запуск проекта (локально)](#запуск-проекта-локально)

---

## Описание

Blogicum — это полноценное веб-приложение блога.
Приложение реализует систему публикаций и комментариев с разграничением прав доступа между пользователями.

---

## Функционал
### Пользователи
- Регистрация и аутентификация
- Создание постов
- Комментирование публикаций
### Управление контентом
- Редактирование постов только автором
- Удаление постов только автором
- Редактирование и удаление комментариев их авторами
### Администрирование
- Django Admin для управления:
  - пользователями
  - постами
  - комментариями

---

## Основные технологии
- Python
- Django
- HTML / CSS
- Bootstrap 5

---

## Запуск проекта локально
1. Клонируем репозиторий.
```bash
git clone https://github.com/GohubSilently/blogicum.git && cd blogicum
```

2. Создаем виртуальное окружение и установливаем заввисимости.
```
python3 -m venv .venv && source .venv/bin/activate
pip install --upgrade pip && pip install -r requirements.txt
```

3. Применяем миграции и запускае проект.
```
cd blogicum && python manage.py migrate
python manage.py runserver
```

4. Проверяем тесты и стилистику.
```
flake8 .
cd .. && pytest
```

---
