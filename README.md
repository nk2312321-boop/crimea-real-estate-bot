# crimea-real-estate-bot
Telegram bot for Crimea real estate подбор 
## What it does
- /start — приветствие и сбор запроса на подбор (город/цель/бюджет)
- Работает через webhook + FastAPI (под деплой на Render)
## Deploy (Render)
1. Add env vars:
   - TELEGRAM_BOT_TOKEN
   - WEBHOOK_SECRET
2. Start command:
   uvicorn main:app --host 0.0.0.0 --port $PORT
3. Set Telegram webhook:
https://api.telegram.org/bot<YOUR_TOKEN>/setWebhook?url=<YOUR_RENDER_URL>/webhook&secret_token=<WEBHOOK_SECRET>
