# Project - Personal Git Server
Docker project under IIEC Rise
This project is based on [Gogs self hosted git server](https://gogs.io/) where you can manage all of your personal repositories.
Configured the Gogs git server inside docker container and created a image which you can find on [Docker hub](https://hub.docker.com/repository/docker/harshgautam/go-git). You can easily lauch a personal git server using docker-compose.yml

[PROOF OF CONCEPT](https://bit.ly/2yWnbGG)

## Requirements
*docker 19.03 or above* that you can find [here](https://www.docker.com/get-started)

*docker-compose 1.25.5 or above* that you can find [here](https://docs.docker.com/compose/install/)

## Run 
In the same directory where docker-compose.yml is, start terminal and run
> docker-compose up -d

To stop
> docker-compose down

### Configure
After running docker-compose.yml, Visit `http://your_server_ip/install` and configure gogs as follows
1. *Database* : sqlite3
2. Remove port from ssh because this doesn't uses ssh for repositories
3. *Domain* : yout_ip
4. *HTTP Port* : 3000
5. *Application URL* : http://your_ip:3000/

Everything else let it be default

Skip the optional e-mail and notification settings, then under Admin Account Settings, choose an admin username and password, and include your email address.
Finally, click Install Gogs, and then log in.

## Preview
* ![Screenshot](https://github.com/harsh-gautam/gogs-git/blob/master/screeshot_1.png)
* ![Screenshot](https://github.com/harsh-gautam/gogs-git/blob/master/screenshot_2.png)
* ![Screenshot](https://github.com/harsh-gautam/gogs-git/blob/master/screenshot_3.png)
* ![Screenshot](https://github.com/harsh-gautam/gogs-git/blob/master/screenshot_4.png)
