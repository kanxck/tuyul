#!/bin/sh

ulang='y'

while [ $ulang = 'y' ];
do
  echo -n "\033[1;32m Sriyus Kamu Mau Instal CpuMiner-Multy(Y/T) : \033[1;0m"
  read pil;
  if [ $pil = 'y' ] || [ $pil = 'Y' ];
  then
      clear
      echo "\033[1;32mInstalling Library\033[1;0m"
      sleep 2
      apt update && apt upgrade -y
      apt-get install git build-essential cmake libuv1-dev libmicrohttpd-dev libssl-dev
      apt-get install -qqy automake
      apt-get install -qqy libcurl4-openssl-dev
      apt-get install -qqy make
      echo "\033[1;32mCloning CpuMiner\033[1;0m"
      sleep 2
      git clone https://github.com/tpruvot/cpuminer-multi
      cd cpuminer-multi
      echo "\033[1;32mGasken Install CpuMiner-multi\033[1;0m"
      sleep 2
      ./build.sh
      echo "\033[1;32mInstall Success Gaes\033[1;0m"
      sleep 2
      exit
  elif [ $pil = 't' ] || [ $pil = 'T' ];
  then
     clear
     echo "\033[1;31mExit.......!\033[1;0m"
     sleep 2
     exit
  else
     clear
     echo "\033[1;36mERROR : Please Correct Your Answer...!\033[1;0m"
     sleep 1
     echo $ulang
     clear
  fi
done
