# Familiarization with Various LAN Network Cables

Understanding the different types of network cables used in Local Area Networks (LAN) is crucial for setting up and maintaining efficient computer networks. Below is a summary of common LAN cable types: Coaxial Cable, Unshielded Twisted Pair (UTP) Cable, and Shielded Twisted Pair (STP) Cable.

---

## 1. Coaxial Cable
<img width="404" height="234" alt="image" src="https://github.com/user-attachments/assets/d1be5f28-75fc-4eb3-8a7d-932db9d6432c" />

### Definition
A coaxial cable is an electrical cable with an inner conductor surrounded by a tubular insulating layer, a metallic shield, and often an insulating outer jacket. It is used for transmitting high-frequency signals.

### Properties
- Consists of a central copper conductor
- Surrounded by a dielectric insulator, metallic shield (braid or foil), and outer insulating sheath
- Impedance commonly 50 or 75 ohms

### Features
- Resistant to electromagnetic interference (EMI)
- Supports relatively high bandwidth
- Used in older Ethernet networks (10Base2, 10Base5), cable television, and broadband internet

### Limitations
- Bulky and less flexible compared to twisted pair cables
- Difficult to install and maintain
- Limited scalability for modern high-speed networks
- More expensive than UTP cables

---

## 2. Unshielded Twisted Pair (UTP) Cable
<img width="1400" height="933" alt="image" src="https://github.com/user-attachments/assets/73e1b56e-d3a7-41b3-8750-c7dccd398b2f" />

### Definition
UTP cable is a type of copper cable that consists of pairs of wires twisted together without any shielding. It is the most common cable used in Ethernet networks.

### Properties
- Made up of 2 to 4 pairs of insulated copper wires twisted together
- No additional shielding against EMI
- Categories include Cat 3, Cat 5, Cat 5e, Cat 6, Cat 6a, Cat 7, and Cat 8

### Features
- Lightweight, flexible, and easy to install
- Cost-effective and widely available
- Supports high data transmission rates (up to 10 Gbps for higher categories)
- Used in telephone wiring and Ethernet networks (10Base-T, 100Base-TX, 1000Base-T, 10GBase-T)

### Limitations
- Susceptible to electromagnetic interference (EMI) and crosstalk
- Maximum cable length limited to 100 meters for Ethernet standards
- Less secure due to lack of shielding

---

## 3. Shielded Twisted Pair (STP) Cable
<img width="288" height="252" alt="image" src="https://github.com/user-attachments/assets/ee845b91-45af-4ffa-b609-cc8ef1f8dc19" />

### Definition
STP cable is similar to UTP but includes additional shielding to protect the transmission from external electromagnetic interference.

### Properties
- Consists of pairs of twisted wires with an additional shielding (foil or braided)
- Shielding can be applied to individual pairs or overall cable

### Features
- Improved protection against EMI and crosstalk
- Suitable for environments with high interference (e.g., factories, data centers)
- Supports similar data rates as UTP cables

### Limitations
- More expensive than UTP cables
- Thicker and less flexible, making installation more difficult
- Requires proper grounding to function effectively

---

## 4. Unguided Transmission (Wireless Media)
<img width="412" height="234" alt="image" src="https://github.com/user-attachments/assets/758cbb6b-0a98-47c7-8e41-9255284d12ff" />
The term "unguided media" refers to wireless transmission (e.g., radio waves, microwaves, infrared).

### Definition
Unguided transmission uses electromagnetic waves to transmit data through air, vacuum, or water, rather than physical cables.

### Properties
- No physical medium; uses air as the transmission medium
- Includes radio, microwave, and infrared communication

### Features
- Allows for wireless communication over short or long distances
- Supports mobile and temporary installations
- Easy to deploy in challenging terrains

### Limitations
- Susceptible to interference, attenuation, and eavesdropping
- Limited bandwidth compared to wired cables
- Security concerns due to broadcast nature

---

## 5. Crimping Tool
<img width="241" height="241" alt="image" src="https://github.com/user-attachments/assets/200976e7-236c-4362-997c-1f7023e7a2cd" />

### Definition
A crimping tool is a hand-held device used to attach connectors (such as RJ-45 or RJ-11) to the ends of network cables by deforming (crimping) the connector around the cable.

### Properties
- Usually made of metal with insulated handles for grip and safety
- Contains slots for different connector sizes (e.g., RJ-45, RJ-11)
- Some versions include wire stripping and cutting functions

### Features
- Essential for creating custom-length network cables
- Ensures proper electrical contact between cable wires and connector pins
- Allows quick and reliable assembly of cable terminations
- Portable and easy to use

### Limitations
- Improper use can lead to faulty or unreliable connections
- Requires some skill and practice to use correctly
- Not suitable for fiber optic cables (specialized tools are required for those)

---

## 6. Connectors: RJ-45 and RJ-11

### RJ-45 Connector
<img width="269" height="269" alt="image" src="https://github.com/user-attachments/assets/80498b9f-5c4d-421a-8eba-3c335b05d2e5" />

#### Definition
RJ-45 (Registered Jack 45) is a standardized physical network interface commonly used for terminating twisted pair cables, primarily in Ethernet networking.

#### Properties
- Has 8 positions and 8 contacts (8P8C)
- Typically used with Cat 5, Cat 6, and Cat 6a UTP/STP cables
- Transparent plastic modular plug

#### Features
- Supports high-speed Ethernet connections (up to 10 Gbps)
- Used for connecting computers, switches, routers, and other network devices
- Provides reliable and secure data transmission

#### Limitations
- Not compatible with telephone cables (which use RJ-11)
- Larger than RJ-11; not suitable for compact installations

---

### RJ-11 Connector
<img width="254" height="254" alt="image" src="https://github.com/user-attachments/assets/9e4e1818-7877-47f4-a3fe-8f7fb9802d99" />

#### Definition
RJ-11 (Registered Jack 11) is a standardized physical network interface typically used for terminating telephone cables.

#### Properties
- Has 6 positions and usually 2 or 4 contacts (6P2C or 6P4C)
- Used primarily with telephone wiring and sometimes with low-speed modem connections
- Smaller than RJ-45

#### Features
- Standard connector for landline telephones
- Easy to install and widely available
- Can be crimped onto telephone cables using a crimping tool

#### Limitations
- Not suitable for Ethernet or high-speed data networks
- Limited to low-bandwidth applications (voice, fax, low-speed data)

---

## Summary Table

| Type/Tool         | Properties                        | Features                       | Limitations                       |
|-------------------|-----------------------------------|--------------------------------|-----------------------------------|
| Coaxial           | Central core, shielded            | EMI resistant, reliable        | Bulky, costly, harder to install  |
| UTP               | Twisted pairs, unshielded         | Flexible, cheap, fast          | EMI/crosstalk, less secure        |
| STP               | Twisted pairs, shielded           | EMI/crosstalk protected        | Expensive, less flexible          |
| Unguided/Wireless | No cable, uses radio waves        | Wireless, mobile               | Interference, security, bandwidth |
| Crimping Tool     | Metal, insulated handles          | Makes custom cables easy       | Skill needed, errors possible     |
| RJ-45 Connector   | 8P8C, modular plug                | High-speed Ethernet, reliable  | Not for telephone, bulkier        |
| RJ-11 Connector   | 6P2C/6P4C, small modular plug     | Telephone standard, easy use   | Not for Ethernet, low bandwidth   |

---
