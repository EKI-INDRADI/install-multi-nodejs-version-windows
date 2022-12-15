# INSTALL MULTI NODEJS VERSION WINDOWS


```bash

https://github.com/coreybutler/nvm-windows
https://github.com/coreybutler/nvm-windows/wiki#manual-installation
https://github.com/coreybutler/nvm-windows/releases


create C:NVM_MANUAL

download zip no-install version save folder & rename to C:\NVM_MANUAL\nvm

add new environment windows

NVM_HOME  C:\NVM_MANUAL\nvm
NVM_SYMLINK C:\NVM_MANUAL\nodejs

Path  = %NVM_HOME%;%NVM_SYMLINK%

or

Path   new
%NVM_HOME%
%NVM_SYMLINK%


create file C:\NVM_MANUAL\nvm\settings.txt

root: C:\NVM_MANUAL\nvm
path: C:\NVM_MANUAL\nodejs
arch: 64
proxy: none



//========== NOTE
change permission folder NVM_MANUAL to all user "full control"
//========== NOTE


command -v nvm

nvm ls-remote | grep -i "latest" 

nvm install 18.12.1
nvm install 16.18.1
nvm install 14.21.1

nvm use 14.21.1  (need run as admin if permission not "full control")

npm --version
node --version

example :

npm i -g nodemon
npm I -g pm2
npm i -g @angular/cli
npm i -g @nestjs/cli


```