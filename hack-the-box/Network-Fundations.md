# Introduction to Networks

---

Networking is the technology that allows devices to connect and communicate with each other by sending and receiving data and sharing resources.

A network consists of interconnected devices, called `nodes`, connected through communication links. Examples of nodes include computers, smartphones, printers, and servers.

## Types of Networks

There are two main types of networks: `LAN` and `WAN`.

### Local Area Network (LAN)

A `Local Area Network (LAN)` connects devices within a small geographical area, such as a home, school, or office.

- Covers a small area.
- Usually managed by one person or organization.
- Provides high data transfer speeds.
- Uses Ethernet cables or Wi-Fi to connect devices.

For example, a home network connects computers, smartphones, and printers to the same local network, allowing them to communicate and share resources.

### Wide Area Network (WAN)

A `Wide Area Network (WAN)` connects networks over large geographical areas, such as cities, countries, or continents.

- Covers large geographical areas.
- Can involve multiple organizations and service providers.
- Generally has lower data transfer speeds than a LAN.
- Uses technologies such as fiber optics and satellite links.

The Internet is the largest example of a WAN, connecting millions of LANs around the world.

## LAN vs WAN

| Characteristic | LAN | WAN |
|---|---|---|
| Size | Small geographical area | Large geographical area |
| Ownership | Usually one person or organization | Multiple organizations or service providers |
| Speed | Generally faster | Generally slower than a LAN |
| Example | Home or office network | The Internet |

## How LANs and WANs Work Together

A LAN can connect to a WAN to communicate with devices and access resources outside its local network.

For example, devices in a home connect to a router, forming a LAN. The router connects to an Internet Service Provider (ISP), which provides access to the Internet through a WAN.

This allows devices within the home network to access websites and online services around the world.

# Network Concepts

---

## OSI Model

The `Open Systems Interconnection (OSI) model` is a conceptual framework that standardizes network communication into seven abstract layers. It helps developers create interoperable network devices and software.

### The Seven Layers

**1. Physical Layer**

Transmits raw bits over a physical medium. It deals with physical connections and hardware, such as Ethernet cables, hubs, and repeaters.

**2. Data Link Layer**

Provides direct data transfer between physically connected nodes. It handles data frames, error detection, and correction. Switches and bridges operate at this layer, using MAC addresses.

**3. Network Layer**

Handles packet forwarding and routing across different networks. It uses logical addressing and IP addresses to determine the path to the destination. Routers operate at this layer.

**4. Transport Layer**

Provides end-to-end communication between applications. It handles segmentation, reassembly, flow control, and error checking.

- `TCP`: Reliable, connection-oriented communication.
- `UDP`: Faster, connectionless communication without guaranteed delivery.

**5. Session Layer**

Establishes, maintains, and terminates communication sessions between applications. It also supports session recovery after interruptions.

**6. Presentation Layer**

Ensures that data sent by one system can be understood by another. It handles data representation, encryption, decryption, and compression.

**7. Application Layer**

Provides network services directly to applications. Common protocols include:

- `HTTP`: Web browsing.
- `FTP`: File transfers.
- `SMTP`: Email transmission.
- `DNS`: Resolves domain names into IP addresses.

---

## TCP/IP Model

The `Transmission Control Protocol/Internet Protocol (TCP/IP) model` is a condensed version of the OSI model, designed for practical network communication over the Internet. It consists of four layers.

### The Four Layers

**1. Link Layer**

Handles physical network connections and data framing. It includes technologies such as Ethernet and Wi-Fi.

This layer corresponds to the Physical and Data Link layers of the OSI model.

**2. Internet Layer**

Manages logical addressing and packet routing across networks. Its protocols include:

- `IP`: Handles addressing and routing.
- `ICMP`: Supports network control and diagnostic messages.

This layer corresponds to the Network layer of the OSI model.

**3. Transport Layer**

Provides end-to-end communication between applications.

- `TCP`: Provides reliable communication.
- `UDP`: Provides faster, connectionless communication.

This layer corresponds to the Transport layer of the OSI model.

**4. Application Layer**

Contains protocols that provide network services to applications, such as HTTP, FTP, and SMTP.

This layer combines the Session, Presentation, and Application layers of the OSI model.

---

## OSI vs. TCP/IP

| OSI Model | TCP/IP Model |
|---|---|
| 7 layers | 4 layers |
| Conceptual framework for understanding network operations | Practical model used for Internet communication |
| Separates Session, Presentation, and Application layers | Combines these three layers into the Application layer |
| Separates Physical and Data Link layers | Combines them into the Link layer |

The OSI model helps explain how networks operate, while TCP/IP provides the practical framework for communication across the Internet.

---

## Network Protocols

`Protocols` are standardized rules that define how data is formatted and processed so devices can communicate over a network.

| Protocol | Function |
|---|---|
| `HTTP` | Transfers web pages. |
| `FTP` | Transfers files between systems. |
| `SMTP` | Transmits email messages. |
| `TCP` | Provides reliable, ordered data transmission. |
| `UDP` | Provides fast, connectionless communication without error recovery. |
| `IP` | Handles packet addressing and routing across networks. |

---

## Network Transmission

`Transmission` is the process of sending data signals through a medium from one device to another.

### Transmission Types

- **Analog:** Uses continuous signals to represent information.
- **Digital:** Uses discrete signals, such as bits, to represent data.

### Transmission Modes

- **Simplex:** Communication occurs in one direction only.
- **Half-duplex:** Communication works in both directions, but not simultaneously.
- **Full-duplex:** Communication works in both directions simultaneously.

### Transmission Media

Transmission media are the physical means used to carry data.

**Wired media:**
- `Twisted pair`: Commonly used in Ethernet networks.
- `Coaxial cable`: Used in cable television and early Ethernet.
- `Fiber optic`: Transmits data using light pulses and supports high-speed communication.

**Wireless media:**
- `Radio waves`: Used by Wi-Fi and cellular networks.
- `Microwaves`: Used in satellite communications.
- `Infrared`: Used for short-range communication, such as remote controls.

# Components of a Network

---

A network consists of different components that work together to connect devices, transmit data, and provide services.

## End Devices

An `end device`, also known as a `host`, is any device that sends or receives data over a network.

Examples:
- Computers
- Smartphones and tablets
- Smart TVs and other IoT devices

## Intermediary Devices

`Intermediary devices` facilitate data transmission between end devices within the same network or across different networks. They forward data packets, manage network traffic, and may include security features.

Examples:
- Routers
- Switches
- Modems
- Access points

### Network Interface Cards (NICs)

A `Network Interface Card (NIC)` is a hardware component that allows a device to connect to a network and send or receive data. Each NIC has a unique `MAC address` used to identify it at the Data Link layer.

NICs can support wired Ethernet or wireless Wi-Fi connections.

### Routers

A `router` forwards data packets between different networks. It operates at Layer 3 (Network Layer) of the OSI model and uses IP addresses to determine where packets should go.

Routers connect networks, manage traffic, and may provide security features.

### Switches

A `switch` connects multiple devices within the same network, typically a LAN. It operates at Layer 2 (Data Link Layer) of the OSI model and uses MAC addresses to forward data to the intended recipient.

Switches help reduce network congestion and improve performance.

### Hubs

A `hub` connects multiple devices within a network segment and broadcasts incoming data to all connected ports, regardless of the destination.

It operates at Layer 1 (Physical Layer) of the OSI model. Hubs are outdated and less efficient than switches.

---

## Network Media and Software Components

Network media and software components provide the connections and rules needed for devices to communicate.

### Cabling and Connectors

`Cabling and connectors` physically link devices and provide the paths through which data travels.

Examples:
- Ethernet cables
- Fiber-optic cables
- `RJ-45` connectors, used to connect Ethernet cables to network devices

### Network Protocols

`Network protocols` are standardized rules that define how data is formatted, transmitted, received, and interpreted across a network.

They cover aspects such as:
- Data segmentation
- Addressing
- Routing
- Error checking
- Synchronization

Examples:
- `TCP/IP`: Used for Internet communication.
- `HTTP/HTTPS`: Used for web traffic.
- `FTP`: Used for file transfers.
- `SMTP`: Used for email transmission.

### Network Management Software

`Network management software` helps administrators monitor, configure, and maintain networks.

Its functions include:
- Performance monitoring
- Configuration management
- Fault analysis
- Security management

### Software Firewalls

A `software firewall` is a security application installed on an individual device. It monitors and controls incoming and outgoing network traffic based on predefined security rules.

Unlike hardware firewalls that can protect entire networks, software firewalls provide protection at the device level. They help block unauthorized connections and suspicious traffic.

---

## Servers

A `server` is a computer designed to provide services and resources to other computers, known as clients, over a network.

Servers can:
- Host websites and applications.
- Provide file and email services.
- Store and manage data centrally.
- Share resources.
- Manage authentication, user access, and permissions.

### Client-Server Model

In the `Client-Server Model`, a client sends a request to a server, and the server processes the request and returns a response.

For example, when accessing a website, a browser sends a request to the web server, which responds with the webpage data.

---

# Network Communication

---

Network communication relies on three main components: `MAC addresses`, `IP addresses`, and `ports`. Together, they help deliver data to the correct device and application.

## MAC Addresses

A `Media Access Control (MAC) address` is a unique identifier assigned to a device's Network Interface Card (NIC). It operates at Layer 2 (Data Link Layer) of the OSI model and is used for communication within a local network.

- Length: 48 bits.
- Format: Hexadecimal, usually represented as six pairs of digits.
- First 24 bits: Identify the manufacturer (OUI).
- Last 24 bits: Identify the individual device.

Switches use MAC addresses to forward data frames to the correct device. `ARP (Address Resolution Protocol)` maps IP addresses to MAC addresses within a local network.

## IP Addresses

An `Internet Protocol (IP) address` is a numerical identifier assigned to a device on an IP network. It operates at Layer 3 (Network Layer) and allows devices to communicate across different networks.

There are two versions:

- `IPv4`: Uses 32-bit addresses, usually written as four decimal numbers separated by dots (e.g., `192.168.1.1`).
- `IPv6`: Uses 128-bit addresses, written in hexadecimal.

Routers use IP addresses to determine where to forward packets. Unlike MAC addresses, IP addresses can change depending on the network and its configuration.

## Ports

A `port` is a number used to direct network traffic to a specific application or service on a device. Ports operate at Layer 4 (Transport Layer) and work with protocols such as TCP and UDP.

Port numbers range from `0` to `65535` and are divided into three categories.

| Category | Range | Description |
|---|---|---|
| Well-known ports | 0–1023 | Reserved for common services and protocols. |
| Registered ports | 1024–49151 | Registered for specific services and applications. |
| Dynamic/Private ports | 49152–65535 | Typically used temporarily by client applications during connections. |

### Common Ports

- `80`: HTTP
- `443`: HTTPS
- `20–21`: FTP
- `1433`: Microsoft SQL Server

## Example: Browsing the Internet

When accessing a website, several steps take place:

1. **DNS Lookup:** The computer resolves the domain name into an IP address.
2. **Data Encapsulation:** The browser generates an HTTP request, which is encapsulated with TCP and destination port information. The destination IP address is also included.
3. **Local Network Delivery:** The computer uses ARP to find the MAC address of its default gateway (router).
4. **Data Transmission:** The frame is sent to the router, which forwards the packet toward the destination IP address. Other routers continue forwarding it across networks.
5. **Server Processing:** The server receives the packet and directs the request to the application listening on the appropriate port.
6. **Response Transmission:** The server sends a response back to the client's temporary port, and the response travels back through the network.


# Dynamic Host Configuration Protocol (DHCP)

---

## Introduction to DHCP

The `Dynamic Host Configuration Protocol (DHCP)` is a network management protocol that automatically configures devices on IP networks.

It allows devices to receive an IP address and other network settings without manual configuration, including:

- IP address
- Subnet mask
- Default gateway
- DNS servers

DHCP simplifies network management, helps prevent IP address conflicts, and reuses addresses when devices disconnect from the network.

## How DHCP Works

The DHCP process is known as `DORA`, which stands for `Discover`, `Offer`, `Request`, and `Acknowledge`.

### DHCP Roles

| Role | Description |
|---|---|
| `DHCP Server` | A network device, such as a router or dedicated server, that manages available IP addresses and network configuration parameters. |
| `DHCP Client` | A device that requests an IP address and other network configuration parameters from the DHCP server. |

### The DORA Process

| Step | Description |
|---|---|
| `1. Discover` | The client broadcasts a DHCP Discover message to find available DHCP servers. |
| `2. Offer` | The DHCP server responds with a DHCP Offer, proposing an IP address to the client. |
| `3. Request` | The client sends a DHCP Request to accept the offered IP address. |
| `4. Acknowledge` | The server sends a DHCP Acknowledge (ACK), confirming the IP address assignment. |

After this process, the client can use the assigned IP address to communicate over the network.

## DHCP Lease and Renewal

DHCP addresses are assigned for a specific period called a `lease time`, rather than permanently.

Before the lease expires, the client attempts to renew it by sending a DHCP Request to the server. If the server approves the renewal, it responds with a DHCP Acknowledge (ACK), allowing the client to continue using the address.

## Example Scenario: Alice's Laptop

1. Alice connects her new laptop to the office network.
2. The laptop sends a DHCP Discover message to find a DHCP server.
3. The server responds with a DHCP Offer, proposing the IP address `192.168.1.10`.
4. The laptop sends a DHCP Request to accept the address.
5. The server sends a DHCP Acknowledge (ACK), confirming the assignment.
6. The laptop can now communicate on the network using `192.168.1.10`.

When the lease approaches expiration, the laptop requests a renewal. If the server approves it, the laptop can continue using the assigned IP address.
