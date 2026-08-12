>Networks allow independent devices to communicate and share information and resources efficiently.

# Major Reasons We Need Networks

## 1. Resource Sharing.

One of the biggest reasons for networking is **sharing resources**.
For example, suppose five computers need a printer.

Without networking:
```Diagram
PC 1 → Printer
PC 2 → Printer
PC 3 → Printer
PC 4 → Printer
PC 5 → Printer
```
You might need multiple printers.

With networking:
```Diagram
PC 1 ──┐
PC 2 ──┤
PC 3 ──┼── Network ── Printer
PC 4 ──┤
PC 5 ──┘
```
All computers can use the same printer.

This is called:

> **Resource sharing**

## 2. Data Sharing

Networks make it easy to transfer information.
```flowChart
Laptop A
   │
   │ File
   ↓
 Network
   │
   ↓
Laptop B
```

```
Examples:

- Sending documents
- Sharing photos
- Database access
- File transfer
- Cloud storage

For example, when you upload a file to Google Drive, your computer communicates with remote servers through networks.
```

## 3. Communication

Networks allow people and systems to communicate.

```Diagram
Person A
   ↓
WhatsApp / Email / Video Call
   ↓
Network
   ↓
Person B
```
```Example
Examples include:

- Email
- Messaging
- Voice calls
- Video conferencing
- Social media
- Collaboration tools
```

## 4. Internet Access

Suppose your laptop is connected to your home Wi-Fi.

```Diagram
Laptop
   ↓
Wi-Fi Router
   ↓
ISP
   ↓
Internet
```

>The network allows your device to communicate with computers and servers around the world.

Without networking, services such as:

- Google
- YouTube
- GitHub
- Cloud platforms
- Online banking
 would not work.

## 5. Centralized Data and Services

>Imagine a company with 500 employees.
  instead of storing everything independently:
  
```Diagram
Employee 1 → Data
Employee 2 → Data
Employee 3 → Data
...
Employee 500 → Data
```

The company can have centralized servers:

```Diagram
             Server
          /    |    \
         /     |     \
       PC1    PC2    PC3
         \     |     /
          \    |    /
          PC4  PC5
```

The server can provide:

- Files
- Databases
- Authentication
- Applications
- Internal websites

This makes management easier.
## 6. Distributed Processing

A large task can be divided among multiple computers.

```Diagram
             Large Task
                 │
       ┌─────────┼─────────┐
       ↓         ↓         ↓
     PC 1      PC 2      PC 3
       │         │         │
       └─────────┼─────────┘
                 ↓
             Final Result
```

This idea is fundamental to:

- Distributed systems
- Cloud computing
- Big data
- Data engineering
- Machine learning infrastructure

For example, systems such as Apache Spark distribute large workloads across multiple machines.

## 7. Reliability

>Network improves the availability.

If the server fails, the service may become unavailable.
```Flow
             Load Balancer
             /     |     \
            ↓      ↓      ↓
         Server1 Server2 Server3
```
**load balancing and advanced networking**.

## 8. Remote Access

>Networks allow you to access resources from another location.

```Diagram
Your Laptop
     │
     │ Internet
     ↓
Remote Server
```
```Diagram
You can remotely:

- Access servers
- Transfer files
- Run commands
- Access databases
- Deploy applications

We'll later see protocols such as **SSH** that make this possible.
```
## 9. Cost Reduction

>Networking can reduce infrastructure costs through resource sharing.

organizations can share:
- Storage
- Servers
- Internet connections
- Applications

# 10. Quick Summary

The major reasons for computer networks are:

|Reason|Example|
|---|---|
|Resource sharing|Shared printer|
|Data sharing|File transfer|
|Communication|Email/video call|
|Internet access|Web browsing|
|Centralized services|Company server|
|Distributed processing|Cluster computing|
|Reliability|Multiple servers|
|Remote access|SSH|
|Cost reduction|Shared infrastructure|
