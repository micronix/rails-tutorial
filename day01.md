# The Internet

[Class Video](https://www.youtube.com/watch?v=HyMxkZ62MEM)

### Internet Protocol

In order for computers to communicate with each other they need a way to know
who is who. When a computer joins a network the computer gets a unique number
that identifies the computer. The system used today in the internet is IP

### IPV4

An ip address is composed of four numbers, each number ranges from 0 to 255.

Examples:

- _192.168.1.1_
- _255.0.0.66_
- _127.0.0.1_

With this system you can assign a total of 255*255*255*255 numbers or 4,228,250,625. There are about 7 billion people alive right now, so not every person in the world would be able to get an ip address.

Exercise

Find your ip address, the process will be different depending on the operating system that you are using. Do it in 3 devices, for me it's my laptop, my phone, and my workspace in cloud9.

### IPV6

IPV6 has a total number of 3.4×10e38 possible numbers. Every grain of sand on earth can have an IP address and you would still have many many more left.

Example IPV6 number 2001:cdba:0000:0000:0000:0000:3257:9652

### Sending Messages

Every communication that happens between computers in the internet happens by sending messages, little packets of information. Each packet has a **From** ip address and a **To** ip address.

### DHCP

How to computers get these IP addresses? Two methods:

- You manually tell the computer what it's IP address is
- Your computer asks another central computer to assign it an IP address

DHCP is the protocol to tell your computer what IP address it should have. The benefits are that you don't manually have to assign it to every computer, and you can prevent two computers from having the same ip address


### DNS

It's hard to remember computer names when they are just numbers, the reason computers use numbers for addresses is because it's way faster than human readable addresses. Some routers have to route 148 million packets per second.

For humans we have a way to identify computers with more readable names. We know the ip address of one computer for example 8.8.8.8 that has a database of human readable names to ip addresses. We send that computer the human readable name and it returns the ip address of that computer. We call these human readable names **hostname**. The central computer that keeps track of all the hostnames and ip addresses is called a **Domain Name Server** or **DNS**.

There is a hirarchy to these names, for example: www.google.com. The top name is com, then google is the host within the com domain, then www is the host within the google.com domain. In order to get the IP address of www.google.com we ask a central server for the ip address of com, then we ask that computer for the ip address of google, then we ask that computer for the ip address of www.

Exercise

Use the nslookup command to find the ip address of different domain names.

- www.cnn.com
- google.com
- www.google.com
- test.io
- codethedream.org
- i.love.pizza.lvh.me

### TCP

Computers can have several programs running at once and they can all send and receive messages. TCP (Transmission Control Protocol) helps with this problem by creating little *"mailboxes"* for each program. Each mailbox is idetified by a number and we call this number a **port**.

When you are sending a TCP message you need two things, you need the IP address and the port. The program that you want to send the message to in that computer will have to check that port for incoming messages.

Exercise: In your browser the format to enter a url is of the format hostname:port, Enter the following in your browser.

- google.com:80
- google.com:443
- google.com:2345

### HTTP

It's a protocol for transfering hypertext. There are several commands that you can send an http server. They are called **HTTP Verbs**. The most common verb is the GET verb. Think of it as a command to get a piece of information from the server.

As an exercise we are going to get the html from stack overflow. Go to the command line and type the follow:

Before using telnet in c9 you have install it by doing the following:

```
sudo apt-get -y update
sudo apt-get -y install telnet
```

```
telnet stackoverflow.com 80
```

This will open a TCP connection to the domain stackoverflow.com on port 80. Then type the following information into the telnet application.

```
 GET /questions HTTP/1.0
 Accept: text/html
 Host: stackoverflow.com
```
You should see html text

Something else to try:

```
telnet codethedream.org 80

GET /about HTTP/1.0
Accept: text/html
Host: codethedream.org
```

### NAT

If you have a router at home you will have an internal ip address and an external ip address. NAT stands for Network Address Translation, all the computers in the network have an IP addresYour computer hands the message to the router, the router then hands the message to the computer you want to communicate,

 ![im](https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Components.PostAttachments/00/00/57/53/22/nat_portmapping.gif)
