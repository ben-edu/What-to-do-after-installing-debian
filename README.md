# What-to-do-after-installing-debian

## Drivers Dell

### Wifi

``` sudo nano /etc/apt/sources.list 
deb http://httpredir.debian.org/debian/ stretch main contrib non-free 
sudo apt-get update && apt-get install firmware-iwlwifi 
sudo modprobe -r iwlwifi
sudo modprobe iwlwifi ´´´

## Software

### Git

``` sudo apt-get install git ´´´

### Enpass 

``` sudo echo "deb https://apt.enpass.io/ stable main" > \   /etc/apt/sources.list.d/ enpass.list
sudo wget -O - https://apt.enpass.io/keys/enpass-linux.key | apt-key add -
sudo apt-get update
sudo apt-get install enpass ´´´


