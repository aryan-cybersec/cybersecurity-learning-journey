# Day 2 - Hub, Switch & Router

## Topics Covered

- Hub
- Switch
- Router
- MAC Address
- IP Address
- CAM Table
- Packet Flow
- Hub vs Switch vs Router

---

# Hub

## What is a Hub?

A hub is a basic networking device that connects multiple computers in a network. It works like a multiport repeater and broadcasts incoming data to every connected device without checking the destination.

### OSI Layer

Physical Layer (Layer 1)

### Characteristics

- Broadcasts data to all devices
- Does not use MAC addresses
- No intelligence
- Half-duplex communication
- Low security
- Rarely used today

### Advantages

- Simple
- Inexpensive
- Easy to install

### Disadvantages

- High network traffic
- Poor security
- Frequent collisions
- Slow performance

---

# Switch

## What is a Switch?

A switch is a networking device that connects devices within the same Local Area Network (LAN). It forwards data only to the intended device using MAC addresses.

### OSI Layer

Data Link Layer (Layer 2)

### Characteristics

- Uses MAC addresses
- Maintains a CAM (MAC Address) Table
- Sends data only to the destination device
- Reduces collisions
- Better security than a hub

### Unknown Unicast Flooding

If a switch does not know the destination MAC address, it floods the frame to all ports except the incoming port. Once the destination replies, the switch learns and stores the MAC address in its CAM table.

---

# Router

## What is a Router?

A router connects different networks and forwards packets using IP addresses. It determines the best path for packets to reach their destination.

### OSI Layer

Network Layer (Layer 3)

### Characteristics

- Uses IP addresses
- Connects different networks
- Routes packets
- Connects LAN to the Internet

---

# Packet Flow

Laptop
↓
Switch
↓
Router
↓
Internet
↓
Web Server

- Laptop creates the request.
- Switch forwards the frame using MAC addresses.
- Router forwards the packet using IP addresses.
- Internet delivers the packet to the destination server.
- The response follows the reverse path.

---

# Hub vs Switch vs Router

| Feature | Hub | Switch | Router |
|---------|------|---------|---------|
| OSI Layer | Layer 1 | Layer 2 | Layer 3 |
| Uses | Electrical Signals | MAC Address | IP Address |
| Forwards Data To | All Devices | Intended Device | Different Networks |
| Security | Low | Medium | High |
| Performance | Slow | Fast | Fast |
