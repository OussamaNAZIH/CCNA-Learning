# 🌐 Internet Protocol Version 4 (IPv4)

**Internet Protocol Version 4 (IPv4)** is the most widely used network layer protocol in computer networks. It provides **logical addressing** and enables devices to communicate across different networks by identifying both the network and the host.

IPv4 operates at **Layer 3 (Network Layer)** of the OSI model.

---

# Key Characteristics

- OSI Layer: **Layer 3 (Network Layer)**
- Address Type: **Logical Address**
- Address Length: **32 bits (4 bytes)**
- Representation: **Decimal notation (derived from binary)**
- Address assignment: Static or Dynamic (DHCP)
- Used for communication between different networks

---

# IPv4 Address Format

An IPv4 address consists of **32 bits**, divided into **4 octets**.

Each octet contains **8 bits (1 byte)**.

### Binary Representation

```text
11000000.10101000.00000001.00000001
```

### Decimal Representation

```text
192.168.1.1
```

```text
192      .168      .1        .1
└─8 bits─┘└─8 bits─┘└─8 bits─┘└─8 bits─┘

Total = 32 bits
```

---

# Network and Host Portions

Every IPv4 address is divided into two parts:

- **Network Portion** → Identifies the network.
- **Host Portion** → Identifies a specific device within that network.

For example:

```text
192.168.1.25/24

Network: 192.168.1
Host: 25
```

> The **subnet mask** or **prefix length (/24, /16, /8, etc.)** determines where the network portion ends and the host portion begins.

---

# Binary and Decimal Conversion

Since computers operate using binary, IPv4 addresses are stored as binary values but displayed in decimal form for easier reading.

### Binary to Decimal

| Binary | Decimal |
|---------|--------:|
| 00000000 | 0 |
| 00000001 | 1 |
| 00001010 | 10 |
| 10000000 | 128 |
| 11000000 | 192 |
| 11111111 | 255 |

### Decimal to Binary

| Decimal | Binary |
|---------:|--------|
| 10 | 00001010 |
| 100 | 01100100 |
| 192 | 11000000 |
| 255 | 11111111 |

---

# Address Space

An IPv4 address uses **32 bits**, which provides:

```text
2³² = 4,294,967,296
```

possible unique IPv4 addresses.

However, not all of these addresses are available for general use because some are reserved for:

- Private networks
- Loopback addresses
- Multicast
- Broadcast
- Special-purpose networking

---

# IPv4 Address Structure

```text
192.168.1.25
│    │   │   │
│    │   │   └── Host
│    │   └────── Host
│    └────────── Network
└─────────────── Network
```

The exact division between the **network** and **host** portions depends on the subnet mask.

---

# Common Private IPv4 Address Ranges

| Network | CIDR |
|---------|------|
| 10.0.0.0 | /8 |
| 172.16.0.0 – 172.31.255.255 | /12 |
| 192.168.0.0 | /16 |

These addresses are used inside private networks and are not routable on the public Internet.

---

# 📌 Key Takeaways

- IPv4 operates at **Layer 3 (Network Layer)**.
- An IPv4 address is a **32-bit logical address**.
- It consists of **4 octets**, each containing **8 bits**.
- IPv4 addresses are displayed in **decimal notation** but stored in **binary**.
- The **subnet mask** determines the **network** and **host** portions of an address.
- IPv4 provides approximately **4.29 billion** unique addresses.