# 🏢 Enterprise Network Design (Three-Tier Architecture)

The **Three-Tier Architecture** is a hierarchical network design model widely used in enterprise networks. It divides the network into three layers, each with a specific role. This approach improves scalability, performance, security, and simplifies network management.

The three layers are:

- 🏛️ Core Layer
- 🏢 Distribution Layer
- 🖥️ Access Layer

---

## 🖥️ Access Layer

The **Access Layer** is the closest layer to end users. It provides network access for devices such as computers, printers, IP phones, wireless access points, and other endpoints.

### Responsibilities

- Connect end devices to the network
- Layer 2 switching
- VLAN assignment
- Port security
- Power over Ethernet (PoE)
- Access Control Lists (ACLs)
- Device authentication (802.1X)

### Typical Devices

- Access Switches
- Wireless Access Points (APs)

---

## 🏢 Distribution Layer

The **Distribution Layer** acts as the boundary between the Access Layer and the Core Layer. It aggregates traffic from multiple access switches and applies network policies.

### Responsibilities

- Inter-VLAN Routing
- Route summarization
- Policy enforcement
- Quality of Service (QoS)
- Access Control Lists (ACLs)
- Load balancing
- Redundancy

### Typical Devices

- Layer 3 Switches (MLS)
- Enterprise Routers

---

## 🏛️ Core Layer

The **Core Layer** is the backbone of the enterprise network. It provides fast, reliable, and highly available connectivity between distribution layers.

### Responsibilities

- High-speed packet forwarding
- High availability
- Redundant paths
- Fast convergence
- Minimal latency

The Core Layer should **avoid complex processing** such as ACLs or packet filtering to maximize performance.

### Typical Devices

- High-performance Layer 3 Switches
- Core Routers

---

# 📊 Three-Tier Architecture Diagram

```text
                    Internet
                        │
                   Edge Router
                        │
                  Firewall / NGFW
                        │
                ┌─────────────────┐
                │   Core Layer    │
                └─────────────────┘
                     │       │
         ┌───────────┘       └───────────┐
         │                               │
 ┌─────────────────┐             ┌─────────────────┐
 │ Distribution    │             │ Distribution    │
 │     Layer       │             │     Layer       │
 └─────────────────┘             └─────────────────┘
        │      │                        │      │
        │      │                        │      │
   ┌────────┐ ┌────────┐          ┌────────┐ ┌────────┐
   │ Access │ │ Access │          │ Access │ │ Access │
   │ Switch │ │ Switch │          │ Switch │ │ Switch │
   └────────┘ └────────┘          └────────┘ └────────┘
      │ │ │         │                 │ │ │
     PCs AP IPP    PCs              PCs AP IPP
```

> **AP = Access Point**  
> **IPP = IP Phone**

---

# 📋 Layer Comparison

| Layer | Main Purpose | Typical Devices |
|--------|--------------|-----------------|
| 🖥️ Access | Connect end devices to the network | Access Switches, Access Points |
| 🏢 Distribution | Aggregate traffic, routing, security policies | Layer 3 Switches, Routers |
| 🏛️ Core | High-speed backbone connecting the network | High-performance Layer 3 Switches, Core Routers |

---

# ✅ Advantages of the Three-Tier Architecture

- Scalable network design
- Easier management and troubleshooting
- Better network performance
- High availability and redundancy
- Improved security through policy enforcement
- Easier network expansion
- Modular design suitable for enterprise environments

---

# 💡 CCNA Exam Tip

Remember the responsibilities of each layer:

- **Access Layer** → Connects end devices.
- **Distribution Layer** → Performs routing and applies network policies.
- **Core Layer** → Provides fast, reliable transport across the enterprise network.

> A common way to remember it is:
>
> **Access = Connect**  
> **Distribution = Control**  
> **Core = Transport**