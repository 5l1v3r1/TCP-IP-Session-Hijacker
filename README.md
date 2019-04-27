# F.A.Q

# TCP-IP-Connection-Intruder
1. Advanced TCP-IP connection session hijacker can intrude into any unencrypted protocols and execute data payload using target credentials stealthly

# LICENSE
EULA

# TCP-IP Connection Intruder
- Interface 
<div align="center">
    <img src="http://oi64.tinypic.com/169rrzn.jpg" width="400px"</img> 
</div>

# TCP-IP Connection Intruder
- In this example, I have caught HTTP plain request & executed data payload using target credentials stealthly
<div align="center">
    <img src="http://oi63.tinypic.com/2ic9jxu.jpg" width="400px"</img> 
</div>


# What is TCP-IP Connection Intruder?
1. It works in NETWORK SWITCHES & HUBS stealthly!
2. It is not MAN IN THE MIDDLE ATTACK!
3. IDS / FIREWALLS will not see it!
4. It is not DNS SPOOFING!
5. It is not ARP or ICMP SPOOFING!

# How it capture requests?
1. It uses data headers using TCP-IP sequence magic

# TCP-IP Session Attack Method
1. At the establishment of a TCP session the client starts by sending a SYN-packet (SYN=synchronize) with an sequence number.
This number is used to assure the transmission of packets in a chronological order. It is increased by one with each packet.
The both sides of the connection wait for an packet with a specified sequence number. The first seq-number for both directions is random.
2. The server responds with an SYN/ACK packet (ACK-acknowledgment) which contains the seq-number of the client+1 and also a own start seq-number. The client confirm everything with an ACK packet including the seq-number of the server+1, after that the session is established.
                +---+       syn seq=x       +---+
                | C | ------------------->  | S |
                | L |                       | E |
                | I |   syn ack=x+1 seq=y   | R |
                | E | <-------------------- | V |
                | N |                       | E |
                | T |    ack=y+1 seq=x+1    | R |
                +---+ --------------------> +---+
                
3. To hijack a session it is required to send a packet with a right seq-number, this is where this tool come to inject payload.
    
# How requests are handled?
1. Web requests are automatically handled by Perl modules.

# Payload
1. TELNET payload is included, as "haroon:hacker" as user/pass for TELNET sessions
2. FTP payload can be added as "useradd haroon passwd hacker" 
3. SMTP payload can be add
4. HTTP specific payload can be add like increasing/adding user or doing something cool with specific parameter

# Increasing Payload
1. Currently, I have injected payload in data section specifically for TELNET sessions running in UNIX platforms
2. When successfully authenitcated as victim, it will automatically add haroon:hacker as user/pass for TELNET sessions
3. More paylaods for HTTP/ FTP/ POP3/ SMTP/ TELNET, can be added in data inject command section
4. It can hack plain HTTP protocols using in banks or open area, 
5. It can hack subdomains plain HTTP, be creative! 

# Error Handling Capability
1. It have built-in capability and I don't think any naive will able to use this software

# Advantages of TCP-IP Connection Intruder
1. It is fully automatic, it doesn't want user to wait and output false positive information but it fully provide useful 
information or no information at all without wasting time
2. It is false negative and false positive free.
3. It is fully powered by Perl
5. Secure your network switches and hubs and understand how this software can inject anything in seconds without
alarming any piece of firewall or IDS

# How-to use it?
1. You should be root in Debian/Kali

# Requirement
1. TCP-IP Connection Intruder runs on any *Nix system
3. TCP-IP Connection Intruder needs Perl

# Contact
mrharoonawan@gmail.com
