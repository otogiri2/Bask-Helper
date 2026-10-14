<div align="center">

# 🎓 Bask Helper

**Telegram-помощник для студентов: расписание, замены, звонки и уведомления в одном боте.**

![Python](https://img.shields.io/badge/Python-3.11+-3776AB?logo=python&logoColor=white)
![Telegram](https://img.shields.io/badge/Telegram-Bot-26A5E4?logo=telegram&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-Database-003B57?logo=sqlite&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-green)

</div>

![Карточка расписания](docs/schedule-card.png)

## Возможности

- регистрация студента по отделению, смене и группе;
- расписание на сегодня и завтра;
- автоматическая загрузка замен;
- официальное расписание звонков;
- уведомления перед началом и окончанием пары;
- карточки расписания и исходные PDF;
- профиль с отдельными настройками уведомлений;
- админ-панель, статистика, синхронизация и рассылки;
- SQLite и защита от повторной отправки уведомлений.

## Быстрый запуск

```powershell
py -3 -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
Copy-Item .env.example .env
python run.py
```

Заполни `BOT_TOKEN` и `ADMIN_IDS` в `.env`. Настоящий токен нельзя публиковать или добавлять в Git.

## Структура

```text
app/        основная логика бота
tests/      автоматические тесты
run.py      точка запуска
bothost.json конфигурация BotHost
```

## Проверка

```powershell
python -m unittest discover -s tests -v
```

## Лицензия

Проект распространяется по лицензии MIT.
