# Simple-Network-Simulation-Lab
A structured network simulation lab using Cisco Packet Tracer that demonstrates the design, configuration, and validation of a basic secure LAN in a star topology. Includes static IP addressing, end-to-end connectivity verification, server firewall configuration, and HTTP service testing.
## 🖥️ Scenario
  
**Network Engineer**: Tega Olomu  
**Company**: SecureNet Solutions  
**Tool**: Cisco Packet Tracer
## 🎯 Lab Objective

- Create a star-topology network using Cisco Packet Tracer  
- Assign static IP addresses to all end devices  
- Verify device-to-device connectivity  
- Configure firewall rules on the server  
- Block ICMP (ping) traffic  
- Allow HTTP traffic to the server
## 🛠️ Network Components

| Device Type       | Quantity | Notes                             |
|-------------------|----------|-----------------------------------|
| PCs               | 3        | End-user devices                  |
| Server            | 1        | Hosts firewall & web services     |
| Cisco Switch      | 1 (2960) | Central connecting device         |
| Cables            | 4        | Copper straight-through cables    |

---

## 🧩 Network Configuration Steps
#### 1. **Create Network Topology**
- Add 3 PCs, 1 Server, and 1 2960 Switch to the workspace
- Connect all devices to the switch using copper straight-through cables (star topology)

#### 2. **Assign IP Addresses**
| Device  | IP Address     | Subnet Mask       |
|---------|----------------|-------------------|
| PC0     | 192.168.0.1    | 255.255.255.0     |
| PC1     | 192.168.0.3    | 255.255.255.0     |
| PC2     | 192.168.0.4    | 255.255.255.0     |
| Server0 | 192.168.0.2    | 255.255.255.0     |

#### 3. **Verify Connectivity**
- Use `ipconfig` to confirm correct IP settings
- Use `ping` to confirm PC ↔ Server connectivity

#### 4. **Send a Simple Test Message (PDU)**
- Use the "Add Simple PDU" tool to verify basic network communication

#### 5. **Configure Server Firewall**
- Enable Firewall in the server’s Desktop tab
- **Block ICMP** traffic (to disable ping)
- **Allow IP** traffic (to enable web services)

#### 6. **Test HTTP Traffic**
- On a PC, open a browser and visit `http://192.168.0.2`
- Server homepage should load if configuration is successful

---

## ✅ Results

- All devices communicated before firewall rules were applied  
- ICMP traffic was blocked after applying firewall restrictions  
- HTTP traffic to the server remained accessible  
- The setup simulates real-world LAN setup with basic security

---
## 📄 Documentation

Full report with step-by-step images is available at:  
### 📄 [Network Lab Full Report (PDF)](https://drive.google.com/file/d/1GI7JK-oCBBmSZzTBrnhlv_UrjSEs_j0V/view?usp=drive_link)

---
