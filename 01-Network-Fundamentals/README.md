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