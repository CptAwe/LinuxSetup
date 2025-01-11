# Linux Terminal

## PS1 prompt

```bash
if [[ ${EUID} == 0 ]] ; then
    PS1='\[\033[01;31m\][\h\[\033[01;36m\] \w\[\033[01;31m\]]\n\$\[\033[00m\] '
else
    PS1='\[\033[01;32m\][\u@\h\[\033[01;37m\] \w\[\033[01;32m\]]\n\$\[\033[00m\] '
fi
```

[Online PS1 generator](https://bash-prompt-generator.org/)

## UNICODE logo

### User

```bash
# Colours
GREEN='\033[0;32m'
NC='\033[0m' # no colour

printf "${GREEN}  ___  ____  ____   __    _    _  ____ \n"
printf "${GREEN} / __)(  _ \(_  _) /__\  ( \/\/ )( ___)\n"
printf "${GREEN}( (__  )___/  )(  /(__)\  )    (  )__) \n"
printf "${GREEN} \___)(__)   (__)(__)(__)(__/\__)(____)\n"
```

### Root

```bash
# Colours
RED='\033[0;31m'
NC='\033[0m' # no colour

printf "${RED} ____  _____  _____  ____ \n"
printf "${RED}(  _ \(  _  )(  _  )(_  _)\n"
printf "${RED} )   / )(_)(  )(_)(   )(  \n"
printf "${RED}(_)\_)(_____)(_____) (__) \n"
```
