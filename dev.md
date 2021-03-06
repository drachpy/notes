### Mac auto attach tmux on iterm2 using "Send text at start"
```
tmux ls && read tmux_session && tmux attach -t ${tmux_session:-default} || tmux new -s ${tmux_session:-default}
```


### AFTER CLEAN INSTALL

```
$ sudo apt-get update && sudo apt-get upgrade
```

### INSTALL PROGRAMS

```
$ sudo apt-get install gcc make linux-headers-`uname -r` vim-nox git gitk kdiff3 python-software-properties curl wget 
```

### INSTALL NODEJS

```
$ curl -sL https://deb.nodesource.com/setup_6.x | sudo -E bash -
$ sudo apt-get install nodejs
```

### INSTALL MONO

```
$ sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
$ echo "deb http://download.mono-project.com/repo/debian wheezy main" | sudo tee /etc/apt/sources.list.d/mono-xamarin.list
$ sudo apt-get update
$ sudo apt-get install mono-complete
```

### INSTALL DOTNET CORE

```
$ sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 417A0893
$ sudo apt-get update
$ sudo apt-get install dotnet-dev-1.0.1 
```

### JAVA

```
$ sudo add-apt-repository ppa:webupd8team/java
$ sudo apt-get update
$ sudo apt-get install oracle-java7-installer
$ sudo update-alternatives --config java
```
