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

# Network Address Translation (NAT)

---

## What is NAT?

`Network Address Translation (NAT)` is a process performed by a router that modifies the source or destination IP addresses in IP packet headers as they pass through the network.

NAT allows multiple devices on a private network to share a single public IP address, helping conserve the limited IPv4 address space.

## Private vs. Public IP Addresses

| Type | Description |
|---|---|
| `Public IP` | A globally unique address assigned by an Internet Service Provider (ISP), used to communicate over the Internet. |
| `Private IP` | An address used within local networks, such as homes, schools, and offices. Private IP addresses are not routable on the global Internet. |

Common private IPv4 address ranges:

- `10.0.0.0 – 10.255.255.255`
- `172.16.0.0 – 172.31.255.255`
- `192.168.0.0 – 192.168.255.255`

## How NAT Works

1. A device on a LAN sends a request using its private IP address.
2. The router replaces the device's private source IP with its own public IP address.
3. The request travels across the Internet to the destination server.
4. The server sends a response to the router's public IP address.
5. The router uses its NAT table to identify the internal device associated with the connection.
6. The router translates the address and forwards the response to the correct device.

For example, a laptop with the private IP `192.168.1.10` can access a website through a router with the public IP `203.0.113.50`.

The router's NAT table tracks the connection, including port mappings, so the response reaches the correct device.

## Types of NAT

| Type | Description |
|---|---|
| `Static NAT` | Maps one private IP address directly to one public IP address. |
| `Dynamic NAT` | Assigns a public IP address from an available pool to a private IP address as needed. |
| `Port Address Translation (PAT)` | Also known as NAT Overload. Allows multiple private IP addresses to share one public IP address by distinguishing connections using unique port numbers. It is commonly used in home and small office networks. |

## Benefits and Trade-Offs

### Benefits

- Conserves the limited IPv4 address space.
- Provides a basic layer of security by not directly exposing the internal network structure.
- Offers flexibility for internal IP addressing schemes.

### Trade-Offs

# Internet Architecture

---

## What is Internet Architecture?

`Internet Architecture` describes how data is organized, transmitted, and managed across networks. Different architectures address different needs, and multiple models can be combined to create hybrid systems.

Each architecture has trade-offs in scalability, performance, security, and manageability.

## Peer-to-Peer (P2P) Architecture

In a `Peer-to-Peer (P2P)` network, each node acts as both a client and a server. Devices communicate directly and share resources such as files, processing power, and bandwidth without requiring a central server to host the data.

A common example is torrenting, where users called `seeders` can upload files for others to download from multiple sources.

### Advantages

- `Scalability`: Adding nodes can increase available resources.
- `Resilience`: Other nodes can continue functioning when one goes offline.
- `Cost distribution`: Storage and bandwidth are distributed among peers.

### Disadvantages

- `Management complexity`: Security policies and updates are harder to manage.
- `Potential reliability issues`: Resources may become unavailable when too many peers leave.
- `Security challenges`: Each node can introduce potential vulnerabilities.

## Client-Server Architecture

In the `Client-Server` model, clients send requests to centralized servers, which process the requests and return responses. For example, a browser requests a webpage from a web server.

### Types of Client-Server Architecture

| Type | Description |
|---|---|
| `Single-Tier` | The client, server, and database reside on the same machine. |
| `Two-Tier` | The client handles the presentation layer, while the server manages the data layer. |
| `Three-Tier` | Separates the presentation layer, application server, and database server. |
| `N-Tier` | Uses multiple tiers to distribute processing and business logic across separate components. |

### Advantages

- `Centralized control`: Easier to manage and update.
- `Security`: Central security policies can be applied.
- `Performance`: Dedicated servers can be optimized for specific tasks.

### Disadvantages

- `Single point of failure`: If the central server fails, clients may lose access.
- `High cost and maintenance`: Requires ongoing operation and expert management.
- `Network congestion`: High traffic can slow down or disrupt connections.

## Hybrid Architecture

A `Hybrid Architecture` combines Client-Server and P2P models. Central servers handle tasks such as authentication and coordination, while data can be transferred directly between peers.

For example, a video conferencing application may use central servers for login and meeting management, while audio and video data travels directly between participants.

### Advantages

- `Efficiency`: Peers share data, reducing server workload.
- `Control`: Central servers can manage authentication, directory services, and indexing.

### Disadvantages

- `Complex implementation`: Requires coordination between centralized and distributed components.
- `Potential single point of failure`: A central server failure may interrupt peer discovery.

## Cloud Architecture

`Cloud Architecture` uses computing infrastructure hosted and managed by third-party providers such as AWS, Azure, and Google Cloud. It provides on-demand access to servers, storage, and applications over the Internet.

Examples include Google Drive and Dropbox, which operate under the `Software as a Service (SaaS)` model.

### Five Essential Characteristics

1. `On-demand self-service`: Users can set up and manage services without human assistance.
2. `Broad network access`: Services are accessible from Internet-connected devices.
3. `Resource pooling`: Resources are shared and allocated dynamically among users.
4. `Rapid elasticity`: Resources can scale up or down according to demand.
5. `Measured service`: Resource usage is tracked for billing.

### Advantages

- `Scalability`: Resources can be added or removed as needed.
- `Reduced cost and maintenance`: The provider manages the hardware.
- `Flexibility`: Services are accessible from anywhere with an Internet connection.

### Disadvantages

- `Vendor lock-in`: Moving to another provider can be complex.
- `Security and compliance`: Third-party data hosting raises privacy concerns.
- `Connectivity`: Requires a stable Internet connection.

## Software-Defined Networking (SDN)

`Software-Defined Networking (SDN)` separates the `control plane`, which decides where traffic should go, from the `data plane`, which forwards the traffic.

In SDN, a centralized software-based controller manages network decisions, while network devices execute its instructions. This allows administrators to adjust network policies and routing through software.

### Advantages

- `Centralized control`: Simplifies network management.
- `Programmability and automation`: Configurations can be changed through software.
- `Scalability and efficiency`: Traffic flows can be optimized dynamically.

### Disadvantages

- `Controller vulnerability`: A controller failure can affect the network.
- `Complex implementation`: Requires specialized skills and software or hardware.

## Key Comparisons

| Architecture | Centralization | Scalability | Typical Use Cases |
|---|---|---|---|
| `P2P` | Decentralized or partially centralized | High as peers grow | File-sharing, blockchain |
| `Client-Server` | Centralized | Moderate | Websites, email services |
| `Hybrid` | Partially centralized | Higher than Client-Server | Messaging apps, video conferencing |
| `Cloud` | Centralized in provider infrastructure | High | Cloud storage, SaaS, PaaS |
| `SDN` | Centralized control plane | High, policy-driven | Datacenters, large enterprises |
- Hosting a public server behind NAT may require additional configuration, such as port forwarding.
- NAT can affect protocols that rely on end-to-end connectivity.
- Adds complexity to network troubleshooting.

  # Wireless Networks

---

## What are Wireless Networks?

A `wireless network` connects devices using radio waves or other wireless signals instead of physical cables. It allows devices such as computers, smartphones, and IoT devices to communicate, share files, and access the Internet.

### Advantages

- `Mobility`: Devices can move within the coverage area.
- `Ease of installation`: Requires less cabling.
- `Scalability`: Adding devices is easier than in wired networks.

### Disadvantages

- `Interference`: Signals can be disrupted by walls, electronics, and atmospheric conditions.
- `Security risks`: Wireless transmissions can be intercepted without proper security measures.
- `Speed limitations`: Wireless connections are generally slower than wired connections of the same generation.

## Wireless Router

A `wireless router` forwards data between networks and provides Wi-Fi connectivity. In homes and small offices, it combines two main functions:

| Function | Description |
|---|---|
| `Routing` | Directs data to its destination within the network or on the Internet. |
| `Wireless Access Point` | Allows devices to connect to the network through Wi-Fi. |

### Main Components

| Component | Description |
|---|---|
| `WAN Port` | Connects the router to the Internet source. |
| `LAN Ports` | Connect wired devices, such as desktop computers and printers. |
| `Antennae` | Transmit and receive wireless signals. |
| `Processor and Memory` | Handle routing and network management tasks. |

## Mobile Hotspot

A `mobile hotspot` allows a smartphone or another hotspot device to share its cellular Internet connection through Wi-Fi.

Other devices, such as laptops and tablets, can connect to it to access the Internet through a cellular network like `4G` or `5G`.

Hotspots usually have a range of a few meters and can significantly drain the battery of the device providing the connection. Access is generally protected by a password.

## Cell Towers

A `cell tower`, also known as a `cell site`, contains antennas and communication equipment that provide cellular coverage over a geographic area called a `cell`.

Mobile devices communicate with towers using radio frequencies. As users move, their devices can switch between towers to maintain connectivity.

### Types of Cell Coverage

- `Macro Cells`: Large towers that provide coverage over several kilometers, making them suitable for rural areas.
- `Micro/Small Cells`: Smaller installations commonly used in urban areas to serve densely populated locations and fill coverage gaps.

Cell towers connect to the core network through backhaul links, typically using fiber optics or microwave links. Base Station Controllers (BSCs) manage multiple towers and help coordinate the transfer of calls and data sessions between cells.

## Frequencies in Wireless Communications

Wireless networks use radio waves at specific frequencies, measured in `Hertz (Hz)`. Different frequencies offer different trade-offs between range, speed, and interference.

| Frequency Band | Characteristics |
|---|---|
| `2.4 GHz` | Used by Wi-Fi standards such as 802.11b/g/n. Provides better wall penetration but is more prone to interference from devices such as microwaves and Bluetooth equipment. |
| `5 GHz` | Used by Wi-Fi standards such as 802.11a/n/ac/ax. Offers faster speeds but has a shorter range than 2.4 GHz. |
| `Cellular Bands` | Used by 4G (LTE) and 5G networks. Frequencies range from around 700 MHz to 2.6 GHz and, for some 5G services, 28 GHz and beyond. |

### Frequency Trade-Offs

- `Lower frequencies`: Generally travel farther but carry less data.
- `Higher frequencies`: Can carry more data but typically have a shorter range.
- `Interference`: Can occur when many devices use the same frequency bands.
- `Frequency regulation`: Government agencies regulate frequency allocations to help organize wireless communications and prevent interference.

# Network Security

---

## What is Network Security?

`Network Security` refers to the measures used to protect network data, applications, devices, and systems from unauthorized access or damage.

Its main goal is to maintain the `CIA Triad`:

| Principle | Description |
|---|---|
| `Confidentiality` | Only authorized users can access the data. |
| `Integrity` | Data remains accurate and unaltered. |
| `Availability` | Network resources remain accessible when needed. |

## Firewalls

A `Firewall` is a hardware device, software application, or combination of both that monitors incoming and outgoing network traffic. It uses predefined rules, known as `firewall policies` or `access control lists (ACLs)`, to allow or block traffic.

Firewalls commonly analyze IP addresses, port numbers, and protocols. They can also log network events and generate alerts about suspicious activity.

### Types of Firewalls

| Type | Description |
|---|---|
| `Packet Filtering Firewall` | Operates at OSI Layers 3 and 4, filtering traffic based on IP addresses, ports, and protocols. |
| `Stateful Inspection Firewall` | Tracks connection states and allows traffic based on established connections. |
| `Application Layer Firewall (Proxy Firewall)` | Operates up to Layer 7 and can inspect traffic content, such as HTTP requests, to block malicious requests. |
| `Next-Generation Firewall (NGFW)` | Combines stateful inspection with features such as deep packet inspection, intrusion detection/prevention, and application control. |

A firewall can be built into a home router or installed as a separate device in a larger network.

## Intrusion Detection and Prevention Systems (IDS/IPS)

`Intrusion Detection Systems (IDS)` and `Intrusion Prevention Systems (IPS)` monitor network traffic or system activity to identify suspicious behavior and potential attacks.

| System | Function |
|---|---|
| `IDS` | Detects suspicious activity and generates alerts but does not block the traffic. |
| `IPS` | Detects suspicious activity and can block or reject malicious traffic in real time. |

### Detection Techniques

- `Signature-Based Detection`: Compares traffic against a database of known exploits.
- `Anomaly-Based Detection`: Identifies activity that differs from normal behavior.

### Types of IDS/IPS

| Type | Description |
|---|---|
| `Network-Based IDS/IPS (NIDS/NIPS)` | Inspects network traffic at strategic points in the network. |
| `Host-Based IDS/IPS (HIDS/HIPS)` | Runs on individual devices and monitors their traffic and system logs. |

IDS/IPS solutions can be placed behind a firewall, in a `DMZ (Demilitarized Zone)`, or directly on endpoint devices.

## Network Security Best Practices

| Practice | Description |
|---|---|
| `Define Clear Policies` | Apply consistent firewall rules based on the principle of `least privilege`, allowing only what is necessary. |
| `Regular Updates` | Keep firewalls, IDS/IPS signatures, and operating systems updated. |
| `Monitor and Log Events` | Review firewall logs, IDS/IPS alerts, and system logs to identify suspicious activity. |
| `Layered Security` | Use `defense in depth`, combining firewalls, IDS/IPS, antivirus, and endpoint protection. |
| `Periodic Penetration Testing` | Test security policies and devices by simulating real attacks. |

## Summary

- `CIA Triad`: Confidentiality, Integrity, and Availability.
- `Firewall`: Monitors traffic and allows or blocks it according to predefined rules.
- `IDS`: Detects suspicious activity and generates alerts.
- `IPS`: Detects and prevents malicious traffic.
- `Signature-Based Detection`: Identifies known threats using attack signatures.
- `Anomaly-Based Detection`: Identifies unusual activity.
- `NIDS/NIPS`: Monitor network traffic.
- `HIDS/HIPS`: Monitor individual hosts and their system activity.
- `Least Privilege`: Allows only the access necessary.
- `Defense in Depth`: Uses multiple security layers to improve protection.


  # Data Flow Example

---

## 1. Accessing the Internet

A laptop connects to a home `Wireless LAN (WLAN)` by selecting the correct network (`SSID`) and authenticating with the required password if `WPA2/WPA3` is enabled. Once connected, `DHCP` handles the laptop's IP configuration.

## 2. DHCP Configuration

Before accessing a website, the operating system checks whether the laptop has a valid IP address.

- `DHCP`: Assigns a private IP address to the laptop, such as `192.168.1.10`.
- `DHCP Acknowledgement`: Provides configuration details, including the subnet mask, default gateway, and DNS server.

## 3. DNS Resolution

The laptop needs to resolve the domain `www.example.com` into an IP address.

1. The laptop sends a `DNS query` to a DNS server.
2. The DNS server returns the corresponding IP address, such as `93.184.216.34`.

## 4. Data Encapsulation and Local Transmission

The browser prepares an HTTP or HTTPS request. The data is encapsulated as it moves through the network layers.

| Layer | Function |
|---|---|
| `Application Layer` | Creates the HTTP/HTTPS request. |
| `Transport Layer` | Adds TCP information, including source and destination ports. HTTP commonly uses port `80`, while HTTPS uses port `443`. |
| `Internet Layer` | Adds IP addresses to create an IP packet. |
| `Link Layer` | Encapsulates the packet in an Ethernet or Wi-Fi frame containing MAC addresses. |

Before sending the frame, the laptop uses its `ARP table` or sends an `ARP request` to discover the router's MAC address. The frame is then sent to the router.

## 5. Network Address Translation (NAT)

The router uses `Network Address Translation (NAT)` to replace the laptop's private IP address with its public IP address for internet communication.

Example:

- Private IP: `192.168.1.10`
- Public IP: `203.0.113.45`
- Destination IP: `93.184.216.34`

The packet travels through the ISP's network and intermediate routers, which use the destination IP address to determine where to forward it.

## 6. Server Receives and Responds

The destination server's firewall checks whether the incoming traffic is allowed. If permitted, the web server software, such as Apache, Nginx, or IIS, processes the request and prepares the webpage.

The server sends a response back through the internet. When the response reaches the home router, NAT maps it back to the laptop's private IP address.

## 7. Decapsulation and Display

The laptop receives the response and removes the network headers and frame information as the data moves up the network layers.

Finally, the browser processes the returned HTML, CSS, and JavaScript and displays the webpage.

## Summary

- `WLAN`: Connects the laptop to the local wireless network.
- `DHCP`: Assigns an IP address and other network configuration details.
- `DNS`: Resolves domain names into IP addresses.
- `Encapsulation`: Wraps data with the information required for network transmission.
- `ARP`: Helps discover the MAC address of the default gateway.
- `NAT`: Maps private and public IP addresses for internet communication.
- `Routers`: Forward packets toward their destination using IP addresses.
- `Firewall`: Filters incoming traffic according to security rules.
- `Decapsulation`: Removes network encapsulation information so the application can process the received data.

**Overall process:** Connect to WLAN → Obtain IP configuration → Resolve DNS → Encapsulate and send the request → Apply NAT → Reach the web server → Receive the response → Decapsulate and display the webpage.
