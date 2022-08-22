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
### Remember the older documentaion show `nodejs --version`
### But the latest is `node --version`

