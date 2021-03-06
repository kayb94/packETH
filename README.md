# packETH  

packETH is GUI and CLI packet generator tool for ethernet. It allows you to create and send any possible packet or sequence of packets on the ethernet link. It is very simple to use, powerful and supports many adjustments of parameters while sending packets. It runs on Linux.   

More information about installation, usage, GUI and CLI version and FAQ can be found here:  

http://packeth.sourceforge.net/packeth/Home.html  

Blog with some use cases:  

https://packeth.wordpress.com  

## INSTALLATION  

### GUI  

git clone https://github.com/jemcek/packETH.git  
cd packETH  
./autogen.sh      (you will need aclocal,autoconf,autoheader and automake installed to run this)   
./configure  
make  
make install  
./packETH   

or download the code from: https://sourceforge.net/projects/packeth/files/  
tar xjvf packETH.(version).tar.bz  
cd packETH  
autoreconf -f -i  (optional in case you get automake version mismatch, missing files etc...)   
./configure  
make  
make install  
./packETH  

### CLI  

cd cli  
make  

## USAGE  

### GUI version  
The usage of the program should be pretty straightforward. As you will see, there are 4 main windows (first four buttons from the left side). I call them:   
- Builder - the page where you build the packet and send it once  
- Gen-b - generator for sending packet currently build inside Builder with many options how to send it  
- Gen-s - generator that allows you to select up to 10 previosly built packets and send them in different manner  
- Pcap window - open a tcpdump/wireshark capture file and load the selected packet into builder  

To send the packets you need the SuperUser rights.  

### CLI version  
Type ./packETHcli -h  for available options.  

## AUTHORS & SUPPORT  

If you get into problems, please feel free to contact me.    

Miha Jemec  
jemcek@gmail.com  
packETH (C) 2003-2018 by Miha Jemec, <jemcek@gmail.com>  
Covered under the GPL.  
