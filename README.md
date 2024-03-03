# On new Linux system install

## Update
### Debian / Ubuntu (apt based)
```
sudo apt update && sudo apt upgrade -y
```

## Install minimum viable tooling
```
sudo apt install curl wget zip unzip git ssh -y
```

## Setup a fancy prompt
```
┌──(13:34)-(fvoland@DESKTOP-T4A7GRR)-[~]
└─$ _
```
### Debian / Ubuntu
Color prompt :
```
PS1='${debian_chroot:+($debian_chroot)}┌──(\A)-(\[\033[01;32m\]\u@\h\[\033[00m\])-[\[\033[01;34m\]\w\[\033[00m\]] $(__git_ps1 "(%s)")\n└─\$ '
```

No color prompt :
```
PS1='${debian_chroot:+($debian_chroot)}┌──(\A)-(\u@\h)-[\w] $(__git_ps1 "(%s)")\n└─\$ '
```

## Register aliases
-
  ```
  echo "alias ll='ls -al'" >> ~/.bash_aliases
  ```

## Create SSH key pair
```
ssh-keygen
```

Register your public key on the remote services you use (github...)
