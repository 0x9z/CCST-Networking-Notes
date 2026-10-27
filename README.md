**TCP vs UDP**
TCP is reliable, uses 3-way handshake, retransmits lost segments,
 and is used for HTTP, FTP, and Email.
 UDP is faster, connectionless, no retransmission, 
used for streaming, DNS, and VoIP.

---

**Encapsulation & PDUs**
Data is encapsulated at each layer — Segment (L4), Packet (L3), Frame (L2), Bits (L1). 
Decapsulation happens in reverse at the receiver.

---

**Web Page Request**
User types URL → DNS resolves domain to IP (UDP 53) 
→ TCP 3-way handshake (port 80/443) → HTTP GET request 
→ Server responds → Browser displays page.

---

**Bandwidth vs Throughput vs Goodput**
Bandwidth is maximum theoretical speed.
 Throughput is actual speed affected by latency and congestion. 
Goodput is only the useful data after removing overhead and retransmissions.
 Bandwidth ≥ Throughput ≥ Goodput.

---

**Cloud & Virtualization**
Cloud delivers IT resources over the internet (Public, Private, Hybrid).
Service models: IaaS, PaaS, SaaS. 
Virtualization runs multiple VMs on one physical server using a Hypervisor.

---

**Network Topologies**
Star uses a central switch (most common). Bus uses one shared cable. 
Ring passes data in a loop. 
Mesh provides redundancy. Full Mesh connects every device to every other. 
PAN, LAN, MAN, WAN are network types by size.

---

**NTP & Stratums**
NTP synchronizes time across devices using UDP port 123. Stratum 0 = atomic/GPS clock. 
Each level gets time from the level above. Stratum 16 = not synchronized.

---

**ICMPv4**
ICMP is a Layer 3 protocol for error reporting and diagnostics. 
Ping uses Echo Request/Reply to test connectivity and measure RTT. 
Traceroute uses TTL increments to discover each hop to the destination.

---

**ICMPv6**
RS/RA handle router discovery and replace DHCP in IPv6 (SLAAC). 
NS/NA handle address resolution and replace ARP in IPv4.

---

**DHCP**
IPv4 DHCP uses DORA — Discover, Offer, Request, Ack. 
If the server is on another network, a DHCP Relay Agent (ip helper-address) forwards the request.
 IPv6 uses SARR — Solicit, Advertise, Request, Reply.

---

**URL Structure**
A URL contains: protocol (http/https), subdomain, domain, path, and query string. 
HTTP = port 80. HTTPS = port 443. Domain is resolved to IP using DNS.

---

**DNS**
DNS resolves domain names to IP addresses using UDP port 53. 
The host checks local cache first, then queries a resolver (e.g. 8.8.8.8), 
which searches Root → TLD → Authoritative servers.

---

**IPv4**
IPv4 uses 32-bit addresses. Classes: A (/8), B (/16), C (/24). 
Private ranges: 10.x, 172.16-31.x, 192.168.x. 
APIPA[Automatic Private IP Addressing] = 169.254.x.x (DHCP failed). 
Loopback = 127.0.0.1.

---

**IPv6**
IPv6 uses 128-bit addresses to solve IPv4 exhaustion.
 Transition: Dual Stack, Tunneling, NAT64. 
SLAAC auto-configures addresses using RA messages. 
No broadcast — only Unicast, Multicast, Anycast. Loopback = ::1.

---

**Media Types**
Copper (UTP/STP) = electrical, max 100m, affected by EMI/RFI. 
Fiber = light pulses, immune to EMI, Single Mode (100km+) / Multimode (2km).
 Wireless = radio waves, affected by interference.

---

**Wireless vs Cellular**
WiFi uses unlicensed spectrum (IEEE 802.11) on 2.4GHz and 5GHz. 
Channels 1, 6, 11 are non-overlapping. 
Cellular uses licensed spectrum, wider coverage, but costs more.

---

**FTP & SFTP**
FTP transfers files using ports 20/21 — no encryption. 
SFTP uses SSH port 22 — encrypted. Commands: dir, get, put, quit.

---
