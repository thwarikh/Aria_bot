## Watch Video (might be old and miss some points but will get you to it) Don't follow video, just use as hint.
https://drive.google.com/file/d/1q5VVCCreOuXsujRzZkBAv12WJ1KZvQ0I/view

## Basic Documentation

* Import the Original Repo
* https://github.com/new/import
* Import Repo https://github.com/out386/aria-telegram-mirror-bot
* Change few file names.
* `aria.sh.example` to `aria.sh`
* In src `.constants.js.example` to `.constants.js`
* Create a Telegram Bot
* Change Token in `.constants.js` on line 2.
* Create a Folder inside you Google Drive, open it and Copy it's ID or create Team/Shared Drive and copy it's folder ID.
* For `https://drive.google.com/drive/folders/1p7pHhSh2yboWePmo53DnVr3xkAYiojP9` `1p7pHhSh2yboWePmo53DnVr3xkAYiojP9` is ID.
* Paste Folder ID in `.constants.js` on line 9.
* Edit `.constants.js` as you need.
* Create your own Google Cloud Credentials or copy from [here](https://github.com/HashHackers/aria-telegram-mirror-bot/client_secret.json) and paste in your repo.
* Start an EC2 AWS Virtual Machine or Your Own Linux Machine. (I use Termiux to connect)
* `sudo apt update`
* `sudo apt upgrade`
* `sudo apt install aria2`
* `curl -sL https://deb.nodesource.com/setup_10.x | sudo -E bash -`
* `sudo apt install nodejs`
* `sudo npm install -g typescript`
* `git clone https://github.com/out386/aria-telegram-mirror-bot`    Change this url to your repo url.
* `cd aria-telegram-mirror-bot`
* `sudo npm install`
* `sudo tsc`
* `sudo bash ./aria.sh`
* It Should Print `Aria2c daemon started`
* `sudo screen` this will keep the Bot online even if you close the SSH connection.
* `sudo npm start`
* Your Bot is Started. Send `/mirror https://mirror.nforce.com/pub/speedtests/10mb.bin` to your Telegram Bot.
* In Terminal Copy the accounts.google.com full url and paste in browser and authenticate your drive.
* Paste the Token you received in terminal.
* Your Bot is active.

## Few Tweeks

* In `aria.sh` on line 9 add `--bt-stop-timeout=600` where 600 is seconds, this will cancel dead torrents after 10 minutes.
* In `aria.sh on line 6 change the number of parallel downloads.
