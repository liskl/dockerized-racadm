# dockerized-racadm
dockerized racadm to allow for universal racadm usage.

[![Build Status](https://drone.liskl.com/api/badges/liskl/dockerized-racadm/status.svg)](https://drone.liskl.com/liskl/dockerized-racadm)

## Assuptions:
	you have a variable named $LOM_PASSWD set in your environment
	you know the ip the the drac your wanting to work with

## Make
docker build .

docker run -it <imagename> -r 192.168.30.XXX -u root -p ${LOM_PASSWD} help
docker run -it <imagename> -r 192.168.30.XXX -u root -p ${LOM_PASSWD} getsysinfo | grep "NIC1 Ethernet

and tons more

