# Sunnee Telegram Bot - Render Hosting

## Deploy
1. Push this folder to GitHub.
2. Create a Render Web Service from the repository, or use `render.yaml`.
3. Set the environment variables listed in `.env.example`.
4. Deploy with:
   Build: `pip install -r requirements.txt`
   Start: `python sunnee.py`

## Security
Do NOT commit `.env` or a real Telegram bot token.
The original hard-coded token has been replaced with `BOT_TOKEN`.

## Database
The bot uses SQLite under `inf/bot_data.db`. For production persistence on Render,
attach persistent storage or migrate the database to a managed database.
