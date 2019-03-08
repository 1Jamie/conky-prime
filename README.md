# conky-prime

Linux system monitor utilizing Conky and Lua with a modern/futuristic design

## Required packages

To operate this requires:
```
Conky		apt install conky-all
gawk		apt install gawk
lua		apt install lua-5.1
```

## Usage

To make use of this you will need to move the .conkyrc and .conky folder into your home director.
For working network gauge you will need to correct the network interface settings in the .conkyrc
which you can find yours by using ifconfig and using the appropriate interface you want to monitor.
After configuring everything you can start the system monitor overlay by running conky in a terminal,
or if you want to run it in the background conky -d to run it as a daemon. 


[![conky-prime=examle.png](https://i.postimg.cc/W4vPCTKW/works-jan.png)](https://postimg.cc/3kn6D53m)
