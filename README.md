# MTProxy
With docker-compose file you can easy install telegram mtproto proxy and configure it.

Also build in watchdog check for update telegram-proxy server and if new version come - update it and restart without any action from you.

# Docker
If you have one, read next, if not:

`curl -sSL https://get.docker.com/ | sh`

install docker-compose
On Ubuntu/Debian:

`sudo apt-get update`

`sudo apt-get install docker-compose`

or

`sudo apt-get -y install python-pip`

`sudo pip install docker-compose`


# Clone repository
`git clone https://github.com/borghei/mtproxy.git`

# Edit config.env
In that file you can configure:
- TAG Value, for promote channel
- Preset SECRET, UP TO 16
- Secret count for generate, UP TO 16
- Workers count

# Change proxy port
By default, proxy start at 1000 port, if you want another - edit **docker-compose.yml**:
- "**1000**:443"

# Start proxy
go to folder with that repository:

`cd mtproxy`

and run:

`docker-compose up -d`

# Get logs and connections info
`docker-compose logs`

# Stop proxy
From repository folder:

`docker-compose down`

# Links
Telegram docker hub: https://hub.docker.com/r/telegrammessenger/proxy/

Source Code: https://github.com/TelegramMessenger/MTProxy
