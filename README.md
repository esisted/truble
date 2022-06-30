# truble
import telebot

bot = telebot.TeleBot('5469309990:AAFHW5xDH71ay5r4nZpE4WKm7SZeHlJlLqw')

@bot.message_handler(commands=['start'])
def start(message):
    bot.send_message(message.chat.id, '<b>Привет</b>', parse_mode='html')

bot.polling(none_stop=True)
