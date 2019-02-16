from chatterbot import ChatBot
from chatterbot.trainers import ListTrainer
import os
bot=ChatBot('Bot')
bot.set_trainer(ListTrainer)
for files in os.listdir('/Users/pawansinghchauhan/assistant/chatterbot-corpus-master/chatterbot_corpus/data/english/'):
    data=open('/Users/pawansinghchauhan/assistant/chatterbot-corpus-master/chatterbot_corpus/data/english/'+files,'r').readlines()
    bot.train(data)
while True:
    message=input("me:")
    if message.strip()!="bye":
        reply=bot.get_response(message)
        print("ChatBot:",reply)
    if message.strip()=="bye":
        print("ChatBot:","bye")
        break
