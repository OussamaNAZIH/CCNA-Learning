# 🏢 Network Topologies

A **network topology** describes the physical or logical arrangement of devices and how they communicate with each other. Choosing the right topology is essential for network performance, scalability, reliability, and cost.

The most common enterprise network topologies are:

- 🚌 Bus Topology
- ⭐ Star Topology
- 🕸️ Full Mesh Topology

---

# 🚌 Bus Topology

In a **Bus Topology**, all devices are connected to a single shared communication cable called the **backbone**.

### Diagram

```text
PC1 ─── PC2 ─── PC3 ─── PC4
        Shared Backbone Cable
```

### Advantages

- ✅ Simple to install
- ✅ Low implementation cost
- ✅ Requires less cabling
- ✅ Suitable for very small networks

### Disadvantages

- ❌ A failure of the backbone cable brings down the entire network
- ❌ Difficult to troubleshoot
- ❌ Performance decreases as more devices are added
- ❌ Limited scalability

### Typical Use

- Small or legacy networks (rarely used in modern enterprise environments)

---

# ⭐ Star Topology

In a **Star Topology**, every device is connected to a central device, usually a **switch**.

### Diagram

```text
          PC1
           │
PC2 ─── Switch ─── PC3
           │
          PC4
```

### Advantages

- ✅ Easy to install and manage
- ✅ Easy to troubleshoot
- ✅ High performance
- ✅ Easy to add or remove devices
- ✅ Failure of one cable affects only one device
- ✅ Highly scalable

### Disadvantages

- ❌ The central switch is a single point of failure
- ❌ Requires more cabling than a bus topology
- ❌ Higher installation cost

### Typical Use

- Enterprise LANs
- Office networks
- Schools and universities
- Data centers

> **Star topology is the most common topology used in modern enterprise networks.**

---

# 🕸️ Full Mesh Topology

In a **Full Mesh Topology**, every device has a direct connection to every other device.

### Diagram

```text
      R1
     /  \
   R2----R3
    \    /
      R4
```

Every router is directly connected to all other routers.

### Advantages

- ✅ Very high reliability
- ✅ Excellent fault tolerance
- ✅ Multiple redundant paths
- ✅ No single point of failure
- ✅ Fast rerouting if a link fails

### Disadvantages

- ❌ Very expensive
- ❌ Large amount of cabling
- ❌ Complex configuration
- ❌ Difficult to scale

### Typical Use

- Internet Service Providers (ISPs)
- Core enterprise networks
- Mission-critical environments
- Data center interconnections

---

# 📊 Topology Comparison

| Topology | Cost | Reliability | Scalability | Performance | Typical Use |
|-----------|------|-------------|-------------|-------------|-------------|
| Bus | ⭐ Low | ⭐ Low | ⭐ Low | ⭐⭐ Medium | Small or legacy networks |
| Star | ⭐⭐ Medium | ⭐⭐⭐ High | ⭐⭐⭐ High | ⭐⭐⭐ High | Enterprise LANs |
| Full Mesh | ⭐⭐⭐ High | ⭐⭐⭐⭐⭐ Very High | ⭐ Low | ⭐⭐⭐⭐⭐ Excellent | ISP & critical networks |

---

# 📌 Key Takeaways

- **Bus Topology** is inexpensive but lacks reliability and scalability.
- **Star Topology** is the standard choice for modern enterprise LANs because it is simple, scalable, and easy to manage.
- **Full Mesh Topology** provides maximum redundancy and reliability but is costly and difficult to scale.