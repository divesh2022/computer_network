
---

## 📊 Overview Table: Classful IP Addressing

| Class | Starting Bits | IP Range                  | Default Subnet Mask | Max Networks | Hosts per Network | Usage Scope             |
|-------|----------------|---------------------------|----------------------|--------------|-------------------|--------------------------|
| A     | 0              | 1.0.0.0 – 126.255.255.255 | 255.0.0.0            | 128          | ~16 million       | Very large organizations |
| B     | 10             | 128.0.0.0 – 191.255.255.255 | 255.255.0.0          | 16,384       | ~65,000           | Medium-sized networks    |
| C     | 110            | 192.0.0.0 – 223.255.255.255 | 255.255.255.0        | 2 million+   | 254               | Small networks           |
| D     | 1110           | 224.0.0.0 – 239.255.255.255 | N/A                  | N/A          | N/A               | Multicast                |
| E     | 1111           | 240.0.0.0 – 255.255.255.255 | N/A                  | N/A          | N/A               | Reserved (Experimental)  |

---

## 🧭 Sample Diagram: Classful IP Network Layout

```
+------------------+       +------------------+       +------------------+
|   Class A        |       |   Class B        |       |   Class C        |
|------------------|       |------------------|       |------------------|
| Network: 10.0.0.0|       | Network: 172.16.0.0|      | Network: 192.168.1.0|
| Subnet: /8       |       | Subnet: /16       |       | Subnet: /24       |
| Hosts: 16M       |       | Hosts: 65K        |       | Hosts: 254        |
+------------------+       +------------------+       +------------------+
        |                        |                        |
        |                        |                        |
   +----------+            +----------+            +----------+
   | Router A |            | Router B |            | Router C |
   +----------+            +----------+            +----------+
        |                        |                        |
   +----------+            +----------+            +----------+
   | Host A1   |           | Host B1   |           | Host C1   |
   +----------+            +----------+            +----------+
```

