**SYNSNOOP: A TCP SYN Flood Attack Detection and Mitigation Mechanism in GNU/Linux Kernel 2.6**


SYNSNOOP is an integrated mechanism for detection and mitigation against the TCP SYN Flood 
Attack. 

The SYNSNOOP mechanism enhances the Linux Kernel 2.6 IP code to support 'SNOOPING' of TCP 
related information for countering DoS attacks, using Shannon Entropy.

It saves the effort of processing all the TCP SYN requests under TCP protocol mechanisms. 
All the traffic analysis is completed even before the initiation of normal IP and TCP 
protocol functionality. 


*Setup Information:*


Replace the following files of the GNU/Linux Kernel Source Code with the corresponding 
SYSNOOP files:

* linux-2.6.x.x/include/net/ip.h
* linux-2.6.x.x/net/ipv4/ip_input.c

Compile the GNU/Linux Kernel Source Code.


*Graphs:*

Bandwidth Measurement of a Normal System under DoS Attack:

![System without SYNSNOOP](https://raw.github.com/sandeepsinghmails/synsnoop/master/images/screenshot1.jpeg)

Bandwidth Measurement of a ‘SYNSNOOP’ System under DoS Attack:

![System with SYNSNOOP](https://raw.github.com/sandeepsinghmails/synsnoop/master/images/screenshot2.jpeg)