# HAQQ_telegram_bot

Бот, который проверяет количество имеющихся токенов ISLM в различных состояниях (Делегировано, Разделегирование, Награды и т. д.) Вы отправляете ему свой адрес haqq, и он возвращает количество токенов, которое у вас есть в каждом статусе.

import logging
import requests
from telegram.ext import Updater, CommandHandler, MessageHandler, Filters

# Change these parameters:
BOT_TOKEN = "4544945444:blFKA7VZn639P6A-OWRqgTnxOeF6i-ckbgo" # Telegram bot token
RPC_ADDRESS = "http://95.216.2.219:12317" # Synced up RPC IP Address
