# JustSaveIt_bot

Телеграм бот скачивальщик c

- YouTube
- YouTube Music
- Instagram
- Facebook
- Twitter
- TikTok
- Вконтакте
- SounCloud
- Deezer
- Jamendo и много других сервисов

# Для обхода ограничения в 50МБ

Нобходимо запустить локальный телеграм сервер
Подробнее тут https://github.com/tdlib/telegram-bot-api

```
./telegram-bot-api.exe --api-id=******** --api-hash=******** --http-port=4200

./telegram-bot-api --api-id=******** --api-hash=******** --http-port=4200

```

До запуска локального сервера необходимо отвязать бота от сервера телеграм
Документация telebot https://pypi.org/project/pyTelegramBotAPI/#using-local-bot-api-sever

```
from telebot import apihelper

bot.log_out()
apihelper.API_URL = "http://localhost:4200/bot{0}/{1}"

```

команды для сервера

```
systemctl status justsavit-bot
systemctl restart justsavit-bot
```
