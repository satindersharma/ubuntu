# ubuntu
Ubuntu related stuff



#### set alias in bashrc 

open it with vi

`vi ~/.bashrc`

or with gedit

`gedit ~/.bashrc`


at the end of the file
add

```bash
# using pip as pip3
alias pip=pip3

# using python as python3
alias python=python3

# using py as python3
alias py=python3
```

```bash
# using pip as pip3
alias pip=pip3

# using python as python3
alias python=python3

# using py as python3
alias py=python3
```
```bash
#Virtualenvwrapper settings:
export VIRTUALENVWRAPPER_PYTHON=/usr/bin/python3
export WORKON_HOME=~/.virtualenvs
export VIRTUALENVWRAPPER_VIRTUALENV=~/.local/bin/virtualenv
source ~/.local/bin/virtualenvwrapper.sh
```
```bash
#Virtualenvwrapper settings: on server
export VIRTUALENVWRAPPER_PYTHON=/usr/bin/python3
export WORKON_HOME=~/.Envs
source /usr/local/bin/virtualenvwrapper.sh
```


## some apps and ubuntu software center are not working(or opening )
this may be the cause due to not installed gnome-software , so just installing it sometime fix the error
run the following

###### clean cache
`sudo apt clean`
###### update the system
`sudo apt update && apt upgrade`
###### install gnome-software
`sudo apt install gnome-software`




#### Add git configuration files to ubuntu
### vi ~/.gitconfig
```
[user]
    name = your-github-username
    email = your-github-email
```



#### Install node
##### https://github.com/nodesource/distributions/blob/master/README.md#debinstall

###### curl -fsSL https://deb.nodesource.com/setup_16.x | sudo -E bash -
###### sudo apt-get install -y nodejs
###### It will install node and npm as well
###### check via `node --version` and `npm --version` and `npx --version`
####### Use sudo if facing any issue
### Remember the older documentaion show `nodejs --version`
### But the latest is `node --version`
##### https://docs.npmjs.com/resolving-eacces-permissions-errors-when-installing-packages-globally

##### chech the dir where it is installed  `npm config get prefix` this will return sothing like this `/home/sharma/.npm-packages`
##### `sudo chown -R $(whoami) /home/sharma/.npm-packages`
##### `sudo chown -R $(whoami) ~/.npm`
##### sometimes `sudo chown -R $USER .`




#### `pip install psycopg2-binary`
#####  `sudo -u postgres psql`
##### `CREATE DATABASE new_db;`
##### `CREATE USER db_user WITH PASSWORD 'Pass123';`

##### `GRANT ALL PRIVILEGES ON DATABASE new_db TO db_user;`
