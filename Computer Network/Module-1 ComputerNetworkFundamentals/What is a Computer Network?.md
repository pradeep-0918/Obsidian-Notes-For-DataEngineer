>[!important]
>Computer can process and store data.
>Data can be represented in the form of 0 and 1(bits).
>computers need some way to communicate with others computers.

# Why do we Computer network?

>All Computer are call it as Node.. 
>Each Node Should be communicate via network to share the resources.

```Diagram
Node  A ─────┐
Node  B ─────┤
Node  C ─────┼──── Network
Node  D ─────┤
Node  E ─────┘
```
For Example:
```Diagram
Computer = House
Data     = Vehicle
Network  = Roads
Router   = Junction
Switch   = Local road intersection
Protocol = Traffic rules
```

> if there is no roads then there is no path between two nodes..
i  if road exist then it can travel house A to House B...

```flow chart
House A
   │
   │ Road
   ↓
Junction
   │
   ↓
House B
```


Similary

>`The network provides a way for information to travel between devices.`

```Diagram
Computer A
     │
     │ Network
     ↓
Computer B
```
# Technical Definition:

>[!important]
>Computer Network is a Collection of Interconnected Computing devices that communicate with each other and exchange data and resources Using Communication Links and Agreed upon Protocols

Break Down:
``
```
Collection 
-> Multiple Devices(Pc,Computer,Tablet,Laptop,Phone,Server,Printer,IOT DEVICES)

Interconnected
-> The devices have some form of connection: Device A to Device B
-> Wired And Wireless there are two types of Connection.

Commmunicate
->Send & recieve.

Exchange data
File
Message
Image
Video
Web page
Database information

Exchange resources

Networks can also allow devices to share:

- Printers
- Storage
- Internet connections
- Servers
- Applications

```

# What actually travels  through a network

>When u send  Word "HELLO" from one device to another device through a network..
>Evenually it coverts info into bits...

```flowchart
Hello
  ↓
Data
  ↓
Binary representation
  ↓
101101001...
  ↓
Network transmission
```

>[!info]
>OSI Model → Data Link → IP → TCP → Application protocols

# Basic Network Diagram

```Diagram
             Network
                │
       ┌────────┴────────┐
       │                 │
   Computer A        Computer B
       │                 │
       └────── Data ─────┘
```

```Flow chart
Laptop
   │
   ↓
Switch
   │
   ↓
Router
   │
   ↓
Internet
   │
   ↓
Web Server
```

# Why network are Very Useful

`Major Purpose Include`

>1. Resource Sharing.(Printer)
>2. data Sharing,(file)
>3. communication,(Email,Messaging,Video calls)
>4.Internet Access,(Many devices can access the Internet through network infrastructure.)
>5.Centralized Services,(Many clients can communicate with a central server:)
>6 Distrubuted Computing.(Multiple computers can cooperate to perform work.)

# Real World Example

When you open a website:
```flowchart
Your Laptop
   ↓
Wi-Fi
   ↓
Router
   ↓
ISP
   ↓
Internet
   ↓
Web Server
  ↓
Website
```

You might think:

> "I just opened a website."

But underneath, **many networking concepts are involved**.

```flow chart
DNS
 ↓
IP
 ↓
Routing
 ↓
TCP
 ↓
TLS
 ↓
HTTP/HTTPS
 ↓
Server
 ↓
Response
```
# Network ≠ Internet

 >A network can be small:
   PC ── Switch ── PC
  The Internet is a **global interconnection of networks**.
```flow chart
Home Network
   ↓
ISP Network
  ↓
Regional Networks
  ↓
Other Networks
  ↓
Data Center
```
So:

> **Internet = network of interconnected networks**..
