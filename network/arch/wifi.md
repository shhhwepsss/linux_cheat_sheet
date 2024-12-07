# Before start
> Make shure your wifi adapter is powered on

# [iwd](https://wiki.archlinux.org/title/Iwd#iwctl)

This little guy(a.k.a iNet wireless daemon) helps to connect to a wireless network 

> The iwd package provides the client program iwctl, the daemon iwd and the Wi-Fi monitoring tool iwmon.

your-wlan-name = name column after device list


# Usefull iwd commands

```
adapter your-wlan-name Powered on 
``` 
Desciption: power on your adapter
```
known-networks list 
``` 
Desciption: shows all networks you have worked with, or just memoized

```
station your-wlan-name scan 
``` 
Desciption: starts scanning available wifi connections

```
station your-wlan-name get-networks 
``` 
Desciption: shows available wifi to connect
```
station your-wlan-name connect SSID(network name)
``` 
Desciption: connects to wifi after enter password in interactive mode
