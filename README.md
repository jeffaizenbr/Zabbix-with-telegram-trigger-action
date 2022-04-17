# Zabbix-with-telegram-trigger-action


## Configure BotFather on telegram and save yout TOKEN

search "BotFather" on telegram
```bash
/start
/newbot
/NAME_BOT
/uSERNAME_BOT
```

## On telegram go to "NAME_BOT" and test
```bash
/start
```
## Get yout ID on telegram "IDBOT" and copy
```bash
/GETID
```
## Go to " zabbix>>Administration>>Media Types>>Telegram " 


on Media Type area, copy your "token" on parameters options

![image](https://user-images.githubusercontent.com/83617973/163733568-973c6182-0e57-4b25-8be2-57125ba221eb.png)


## Go to " zabbix>>configuration>>actions>>trigger actions and create a action

![image](https://user-images.githubusercontent.com/83617973/163733635-0f04d2a7-309c-47e7-ac1e-3de96f19eff7.png)


![image](https://user-images.githubusercontent.com/83617973/163733646-ea7e8c69-ac11-45cf-bc33-bd44f6d4ca7d.png)


![image](https://user-images.githubusercontent.com/83617973/163733684-5007a939-6b4c-4bd5-bb49-47e0d7d4222e.png)


## On Custom messages put the example below

Subject
```bash
{TRIGGER.STATUS}: {EVENT.NAME}
```
Message
```bash
Problema iniciado as : {EVENT.TIME} data {EVENT.DATE}
Ultima Coleta: {ITEM.LASTVALUE}
Host: {HOST.NAME}
Severidade: {EVENT.SEVERITY}
ID: {EVENT.ID}
{TRIGGER.URL}
```
