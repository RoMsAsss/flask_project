# flask_project
# PixelQuest - Игровая платформа на Flask и Pygame

🚀 **PixelQuest** - это веб-платформа для запуска пиксельных игр с возможностью онлайн-лидербордов, профилей игроков и чата.

## 🔥 Особенности

- 🎮 Запуск игр прямо в браузере
- 📊 Система рейтингов и достижений
- 💬 Чат между игроками
- 🏆 Лидерборды
- 🛠️ Простой API для добавления своих игр

## 🛠 Технологии

- **Backend:** Flask (Python)
- **Frontend:** Bootstrap 5
- **Игровой движок:** Pygame
- **База данных:** SQLite (Flask-SQLAlchemy)
- **Реальный времени:** Flask-SocketIO

## 🚀 Быстрый старт

### Установка зависимостей
```bash
pip install -r requirements.txt
Запуск сервера
bash
Copy
python app.py
Откройте в браузере: http://localhost:5000

📂 Структура проекта
pixelquest/
├── app.py                  # Основное приложение
├── config.py               # Конфигурация
├── requirements.txt        # Зависимости
├── static/
│   ├── css/                # Стили
│   ├── js/                 # Скрипты
│   ├── games/              # Игры на Pygame
│   └── screenshots/        # Скриншоты
├── templates/              # HTML шаблоны
└── README.md
📝 Как добавить свою игру?
Создайте файл игры в формате .py в папке static/games/

Зарегистрируйте игру в app.py:

python
Copy
games.append({
    "id": 3,
    "name": "Моя игра",
    "description": "Описание игры",
    "file": "my_game.html"  # HTML-обертка для WASM
})
