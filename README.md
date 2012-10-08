Raspberry Pi GPIO Google Talk Bot interface based on njsbot project
------------------
This idea for this project is to extend the [https://github.com/nneves/Raspberrypi_GPIO](https://github.com/nneves/Raspberrypi_GPIO "github.com/nneves/Raspberrypi_GPIO") capabilities and add support to remote control RaspberryPi GPIOs via Google Talk Bot (XMPP) text commands.

To make things simpler and isolated, the Google Talk Bot will run independently from the origial project, using REST (and maybe latter websockets) to SET/RESET the RaspberryPi GPIOS.

(Work In Progress ...)

Install and run
------------------
How to compile node.js on a RaspberryPi
https://github.com/nneves/Raspberrypi_NodeJS

Install the necessary Linux Debian libraries
```bash
sudo apt-get install openssl libssl-dev libexpat1-dev 
```

Install Node.js necessary packages
```bash
git clone git://github.com/nneves/Raspberrypi_GPIO_njsbot.git

cd Raspberrypi_GPIO_njsbot

npm install
```

Run Google Talk Bot
```bash
node app.js localhost 8081

or (for quick testing)

npm start
```

Gtalk/XMPP original source code
------------------
Google Talk Bot code ported from the njsbot project:
The bot is documented at [njsbot.simonholywell.com](http://njsbot.simonholywell.com "njsbot.simonholywell.com").

Released under a [BSD license](http://en.wikipedia.org/wiki/BSD_licenses).

License
------------------
Copyright (C) 2012 Nelson Neves

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU Affero General Public License as
published by the Free Software Foundation, either version 3 of the
License, or any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU Affero General Public License for more details.

You should have received a copy of the GNU Affero General Public License
along with this program.  If not, see http://www.gnu.org/licenses/agpl-3.0.html