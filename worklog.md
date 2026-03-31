---
Task ID: 1
Agent: main
Task: Создание мини веб приложения (Telegram Mini App) для анкет на доп задания

Work Log:
- Инициализировал fullstack dev environment (Next.js 16 + TypeScript + shadcn/ui)
- Создал API маршрут /api/submit — принимает данные формы, валидирует, отправляет через Telegram Bot API
- Создал страницу с формой анкеты (page.tsx) с полями: имя, username, тип задания, описание, бюджет, срок, контакты
- Интегрировал Telegram WebApp SDK — авто-определение юзера, pre-fill полей, закрытие после отправки
- Обновил layout.tsx — подключил telegram-web-app.js script, русская локаль
- Добавил .env.example с переменными BOT_TOKEN и ADMIN_CHAT_ID
- Lint прошёл без ошибок, dev server работает корректно

Stage Summary:
- Приложение готово и работает по адресу /
- Форма мобильного дизайна в стиле Telegram Mini App
- API отправляет анкеты админу через Telegram Bot API
- Требуются переменные окружения: BOT_TOKEN и ADMIN_CHAT_ID
