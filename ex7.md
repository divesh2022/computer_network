---

## 🧠 Experiment Title: Subnet Planning and Its Implementation

---

### 🎯 Aim
To design and implement a subnetting scheme for a given IP network, ensuring optimal utilization of IP addresses, enhanced network segmentation, and improved security and performance.

---

### 🧰 Requirements

#### Hardware Components
- One or more networked computers or laptops
- Network switch or router (Layer 3 preferred)
- Ethernet cables (Cat5e/Cat6)
- Network interface cards (NICs)
- Server (optional, for DHCP or DNS configuration)

#### Software Tools
- IP subnet calculator (online or CLI-based)
- Packet tracer or network simulation software (e.g., Cisco Packet Tracer)
- Operating system with networking utilities (Windows/Linux)
- Text editor for documentation

---

### 📚 Theory (Detailed)

Subnetting is the process of dividing a larger IP network into smaller, manageable subnetworks (subnets). It enhances routing efficiency, improves network security, and allows better utilization of IP address space.

#### Key Concepts:
- **IP Addressing**: IPv4 addresses are 32-bit numbers divided into four octets. Subnetting modifies the default classful boundaries using subnet masks.
- **Subnet Mask**: Determines the network and host portions of an IP address. For example, a /24 mask (255.255.255.0) allows 256 addresses, with 254 usable hosts.
- **CIDR Notation**: Classless Inter-Domain Routing uses suffixes like /26 or /30 to denote subnet sizes.
- **VLSM (Variable Length Subnet Masking)**: Allows different subnet sizes within the same network, optimizing address allocation.
- **Broadcast and Network Addresses**: Each subnet has a reserved network address (first IP) and broadcast address (last IP), which cannot be assigned to hosts.

#### Benefits of Subnetting:
- Reduces broadcast traffic
- Enhances security by isolating segments
- Simplifies troubleshooting
- Enables hierarchical addressing

---

### 🛠️ Procedure (Brief)

1. **Analyze Requirements**: Determine the number of required subnets and hosts per subnet.
2. **Choose Base Network**: Select a suitable IP range (e.g., 192.168.1.0/24).
3. **Calculate Subnets**: Use subnet calculator or manual binary method to derive subnet masks and ranges.
4. **Assign IPs**: Allocate IPs to devices based on subnet plan.
5. **Configure Devices**: Set IP addresses, subnet masks, and gateways on routers/switches and end devices.
6. **Test Connectivity**: Use `ping`, `tracert`, or simulation tools to verify subnet isolation and routing.
7. **Document**: Record subnet plan, IP assignments, and topology for future reference.

---

### ⚠️ Precautions

- Avoid overlapping subnets to prevent routing conflicts.
- Reserve IPs for gateways, servers, and future expansion.
- Ensure subnet masks are correctly configured on all devices.
- Use secure passwords and access controls on routers/switches.
- Backup configuration files before making changes.

---

### ✅ Result

Successfully planned and implemented a subnetting scheme for the given IP network. Devices within each subnet communicated effectively, and inter-subnet routing was verified using gateway configuration. The network was segmented for improved performance and scalability.

---

| Subnet | Subnet Mask     | Number of Hosts |
|--------|------------------|------------------|
| A      | 255.0.0.0        | 16,777,214       |
| B      | 255.128.0.0      | 8,388,606        |
| C      | 255.192.0.0      | 4,194,302        |
| D      | 255.224.0.0      | 2,097,150        |
| E      | 255.240.0.0      | 1,048,574        |
| F      | 255.248.0.0      | 524,286          |
| G      | 255.252.0.0      | 262,142          |
| H      | 255.254.0.0      | 131,070          |
| I      | 255.255.0.0      | 65,534           |
| J      | 255.255.255.0    | 254              |
| K      | 255.255.255.252  | 2                |

| Subnet | IP Address   | Router IP     |
|--------|--------------|---------------|
| A      | 172.16.0.0   | 172.16.0.1    |
| B      | 172.16.1.0   | 172.16.1.1    |
| C      | 172.16.2.0   | 172.16.2.1    |
| D      | 172.16.3.0   | 172.16.3.1    |

| Subnet Name | Subnet Address | Description         |
|-------------|----------------|---------------------|
| Subnet A    | 195.70.26.0     | Connected to Server |
| Subnet B    | 195.70.27.0     | End Users           |
| Subnet C    | 195.70.28.0     | Application Clients |

<img width="1054" height="610" alt="image" src="https://github.com/user-attachments/assets/e614a543-e8d4-431b-ab1d-bc8c6e5bd119" />

