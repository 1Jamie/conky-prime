# conky-prime
Linux system monitor utilizing Conky and Lua with a modern/futuristic design

## Featured in display/overlay

### Time
Time and date both digital and analog with dials and circle indicators

### Network
Network ip addresses for both Ethernet and Wifi (need to set proper interface names)
Domain name (full)
Current network speeds with dial monitor
Current open connections (Incoming and Outgoing)

### CPU/Memory/Storage
CPU overall package usage and individual core/thread usage in dial monitor (up to 8 threads currently) 
Ram usage in percent with dial monitor
System uptime
Number of processes
Number of running processes
Current top processes and percent usage on cores/threads (top 9)
Current usage of storage space, percent and dial

[![conky-prime=examle.png](https://i.postimg.cc/NG44dcGC/conky-prime.png)(https://postimg.cc/9zDZfs7y)

## Required packages

To operate, this requires:
```
net tools	apt install net-tools
Conky		apt install conky-all
Gawk		apt install gawk
Lua		apt install lua5.1
Cairo		apt install libcairo2-dev
```

## Usage

To make use of this you will need to move the .conkyrc and .conky folder into your home director.
For working network gauge you will need to correct the network interface settings in the .conkyrc
which you can find yours by using ifconfig and using the appropriate interface you want to monitor.
After configuring everything you can start the system monitor overlay by running conky in a terminal,
or if you want to run it in the background conky -d to run it as a daemon. 

if you have more cores/threads than shown on ui you can go into /.conky/conky_dashboard.lua and uncomment the lines (lines  177-236)  for cores/threads 5-8


