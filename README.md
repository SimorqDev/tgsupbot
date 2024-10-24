# Telegram Support Bot
Telegram Support Bot for technical support of users. There are three types of panels:

Main - it is intended for users who will create and view their requests through the panel.
Panel for technical support staff. Access to this panel can be obtained by entering the password issued by the administrator. In this panel, the support agent can view and respond to all user requests.
Admin panel - is needed to add and remove support staff, generate / delete access passwords, and also to disable the bot.
And also a control panel for the web for Admin and Agents has been developed

## Requirements
- pyTelegramBotAPI
- pymysql
## Installation

#!

#! nano /etc/systemd/system/lectorientb-bot.service

#! 

[Unit]
Description=Write some description

[Service]
Type=simple
User=root
WorkingDirectory={{root to bot folder}}
Environment=PYTHONPATH={{root to bot folder}}/{{Environments folder name}}
ExecStart={{root to bot folder}}/{{Environments folder name}}/bin/python bot.py
Restart=on-failure
[Install]
WantedBy=multi-user.target

#!
sudo systemctl daemon-reload
service lectorientb-bot start
service lectorientb-bot status
#! if you need stop bot :
service lectorientb-bot stop
#! if you need restart bot :
service lectorientb-bot restart

## Screenshot

## Start








