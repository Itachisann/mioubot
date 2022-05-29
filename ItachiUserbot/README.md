# Itachi Userbot

Fully async userbot built using the basics of [TG-Userbot][tguserbot] based on [Telethon][telethon] library

# 

## Requirements:

* Python 3.7.3 or above.
* Optional Telegram [API Key][tg-apps] (App ID and App Hash).

## How to install:

Clone the repository on your self host and open the new directory.

```sh
$ git clone https://github.com/Itachisann/ItachiUserbot && cd ItachiUserbot
```

> (Optional) Edit the config.ini using Nano or a text Editor and put your APP ID and APP HASH.
```sh
$ nano config.ini
```

Install all the requirements using pip.

```sh
$ pip3 install --user -r requirements.txt
```

Run the userbot and have fun!

```sh
$ python3 -m userbot
```
# 

## Developing
To add extra plugins and functions, simply add the code into [userbot/plugins](userbot/plugins). Each file
that is added to the `plugins` directory. Here's an example
```python
from userbot import client
from userbot.core.events import NewMessage

@client.createCommand(command=("example"),outgoing=True, regex=r"example(?: |$)(.+)?$")
async def module_name(event: NewMessage.Event) -> None:
    await event.edit(
        "This is an example!"
    )
```
# 
## Inspiration and Credits:

* [TG-Userbot][tguserbot]
* [Telethon][telethon]
* [ThunderUserbot](https://github.com/Thundergang)

## Copyright & License

- Copyright (C) 2021 [Itachisann](https://github.com/Itachisann).
- Licensed under the terms of the [GNU General Public License v3.0 or later (GPLv3+)](LICENSE).


































[//]: # (Comment)
   [telethon]: <https://github.com/LonamiWebs/Telethon/>
   [tguserbot]: <https://github.com/TG-UserBot/TG-UserBot>
   [tg-apps]: <https://my.telegram.org/apps>
