# 🌐 Network Fundamentals

## What is a Network?

A **computer network** is a group of **two or more devices** connected together to exchange data and share resources, such as files, printers, or Internet access.

Common network devices include:

- 💻 Computers
- 🖥️ Servers
- 📱 Mobile devices
- 🖨️ Printers
- 🌐 Routers
- 🔀 Switches

---

## Network Types

Networks can be classified based on their geographical size.

### 🏢 Local Area Network (LAN)

A **Local Area Network (LAN)** connects devices within a limited geographic area, such as:

- A home
- An office
- A school
- A university campus

Characteristics:

- High-speed communication
- Usually owned and managed by a single organization
- Uses **switches** to connect devices
- May use a **router** to connect multiple LANs or provide Internet access

### Example

```text
        Internet
            │
         [Router]
            │
       ┌────┴────┐
       │ Switch  │
       └────┬────┘
        │   │   │
       PC1 PC2 Printer
```

---

### 🌍 Wide Area Network (WAN)

A **Wide Area Network (WAN)** connects multiple LANs over large geographic distances, such as different cities or countries.

Characteristics:

- Covers large geographical areas
- Uses the Internet or leased communication links
- Requires an **Internet Service Provider (ISP)**
- Connects multiple routers and networking devices

### Example

```text
Office A LAN
     │
 [Router]
     │
===== Internet =====
     │
 [Router]
     │
Office B LAN
```

---

## Comparison

| Feature | LAN | WAN |
|---------|-----|-----|
| Coverage | Small area | Large area |
| Speed | High | Lower than LAN |
| Ownership | Private | ISP / Multiple organizations |
| Main Devices | Switches, Router | Routers, ISP infrastructure |
| Example | School, Office | Internet |

---

## Key Takeaways

- A network allows devices to communicate and share resources.
- A **LAN** connects devices in a small area.
- A **WAN** connects multiple LANs over long distances.
- Routers connect different networks, while switches connect devices within the same LAN.


# 🖧 Network Components

A computer network consists of several devices that work together to enable communication between hosts.

---

## 🌐 Router

A **router** is a Layer 3 (Network Layer) device that connects different networks and forwards IP packets to their correct destinations.

### Responsibilities

- Connect multiple networks
- Forward IP packets
- Determine the best path using a routing table
- Provide Internet connectivity

> **Note:** Each router interface creates a separate **broadcast domain**.

### Example

```text
LAN A
   │
PC ── Switch ── Router ── Internet
```

---

## 🔀 Switch

A **switch** is a Layer 2 (Data Link Layer) device that connects multiple devices within the same Local Area Network (LAN).

### Responsibilities

- Connect end devices within a LAN
- Forward frames using MAC addresses
- Reduce collisions by providing dedicated communication links
- Improve network performance

### Example

```text
        Switch
      ┌──┼──┬──┐
      │  │  │  │
     PC1 PC2 PC3 Printer
```

---

## ⚡ Multi-Layer Switch (MLS)

A **Multi-Layer Switch (MLS)**, also known as a **Layer 3 Switch (L3 Switch)**, combines the capabilities of both a switch and a router.

### Features

- Performs Layer 2 switching
- Performs Layer 3 routing
- Supports Inter-VLAN Routing
- Provides high-speed routing inside enterprise networks

### Common Uses

- Campus networks
- Enterprise networks
- Data centers

---

## 🔥 Firewall

A **firewall** is a network security device that monitors and filters incoming and outgoing traffic based on predefined security rules.

### Responsibilities

- Protect the internal network
- Block unauthorized access
- Allow only permitted traffic
- Enforce security policies

### Example

```text
Internet
    │
Firewall
    │
Internal Network
```

---

## 🛡 Intrusion Prevention System (IPS)

An **Intrusion Prevention System (IPS)** is a security device that inspects network traffic in real time to detect and prevent malicious activities.

### Responsibilities

- Perform **Deep Packet Inspection (DPI)**
- Detect network attacks
- Block malicious traffic automatically
- Protect against known threats

---

## 🚀 Next-Generation Firewall (NGFW)

A **Next-Generation Firewall (NGFW)** combines the functionality of a traditional firewall with advanced security features such as an Intrusion Prevention System (IPS).

### Features

- Firewall capabilities
- Intrusion Prevention System (IPS)
- Deep Packet Inspection (DPI)
- Application awareness
- URL filtering
- Malware protection

> **NGFW = Firewall + IPS + Advanced Security Features**

---

# 📡 Wireless & Network Management Components

Modern enterprise networks include devices that provide wireless connectivity, centralized management, automation, and analytics.

---

## 📶 Access Point (AP)

An **Access Point (AP)** is a network device that provides **wireless connectivity** to client devices.

Unlike a switch, which connects devices using Ethernet cables, an access point allows devices to communicate over **Wi-Fi**.

### Responsibilities

- Provide wireless network access
- Connect wireless devices to the wired LAN
- Extend wireless network coverage
- Support multiple wireless clients

### Example

```text
          Laptop
             📶
Phone 📶     AP      📶 Tablet
             │
          Switch
             │
          Router
             │
          Internet
```

---

## 🎛️ Wireless LAN Controller (WLC)

A **Wireless LAN Controller (WLC)** is a centralized device used to manage multiple Access Points (APs).

Instead of configuring each AP individually, administrators configure them from a single controller.

### Responsibilities

- Centralized AP management
- Wireless security configuration
- Firmware updates
- Client authentication
- Roaming management

### Benefits

- Simplifies wireless network administration
- Provides consistent configurations
- Improves scalability

---

## ☁️ Cisco DNA Center

**Cisco DNA Center** is Cisco's centralized network management and automation platform.

It provides a graphical interface (GUI) to design, configure, monitor, and automate enterprise networks.

### Main Features

- 📊 Network analytics
- 🤖 Network automation
- 🖥️ Centralized management
- 📈 Performance monitoring
- 🔒 Security policy management
- ⚙️ Device provisioning

Although it is specialized networking software, Cisco DNA Center runs on dedicated hardware and acts as the central management platform for the network.

---

## 💻 Clients

A **client** is an end device that connects to a network to consume or generate data.

Examples include:

- Desktop computers
- Laptops
- Smartphones
- Tablets
- Printers
- IP phones

Clients communicate with servers and other devices through the network infrastructure.

---

## 🖥️ Servers

A **server** is a computer or device that provides services, resources, or data to other devices on a network, known as **clients**. Servers are designed to handle multiple requests simultaneously and operate continuously to ensure services remain available.

Unlike a regular personal computer, a server typically includes more powerful hardware, such as:

- High-performance processors (CPUs)
- Large amounts of memory (RAM)
- High-capacity and redundant storage (RAID)
- Multiple network interfaces
- Reliable power supplies
- Specialized server operating systems (e.g., Windows Server, Linux)

### Common Server Types

- 🌐 Web Server
- 📁 File Server
- 🗄️ Database Server
- 📧 Mail Server
- 🔒 Authentication Server
- ☁️ Cloud Server

---

# 📌 Summary

| Device | OSI Layer | Main Function |
|---------|-----------|---------------|
| Router | Layer 3 | Connects different networks and routes IP packets |
| Switch | Layer 2 | Connects devices within the same LAN |
| Multi-Layer Switch | Layer 2 & 3 | Switching and routing in one device |
| Firewall | Layer 3–7 | Filters and secures network traffic |
| IPS | Layer 3–7 | Detects and blocks network attacks |
| NGFW | Layer 3–7 | Firewall with integrated IPS and advanced security |
| Access Point (AP) | Provides wireless network connectivity |
| Wireless LAN Controller (WLC) | Centrally manages multiple Access Points |
| Cisco DNA Center | Centralized network management, automation, analytics, and monitoring platform |
| Client | End device that sends and receives data over the network |


