# 🌐 Rapid Spanning Tree Protocol (RSTP) – Cisco Packet Tracer

## 📌 Project Overview

This project demonstrates the implementation of **Rapid Spanning Tree Protocol (RSTP)** using Cisco Packet Tracer.

The main purpose of this lab is to understand how RSTP prevents network loops, provides redundancy, and enables faster network convergence compared to traditional Spanning Tree Protocol (STP).

This project is part of my **CCNA Hands-on Networking Practice**.

## 🎯 Project Objectives

- Understand Rapid Spanning Tree Protocol (RSTP).
- Configure RSTP on Cisco switches.
- Understand Root Bridge election.
- Identify Root Ports, Designated Ports, and Alternate Ports.
- Understand RSTP port states.
- Prevent Layer 2 switching loops.
- Improve network redundancy and convergence.
- Verify RSTP using Cisco IOS commands.

## 🖥️ Network Topology

The network topology consists of interconnected Cisco switches with redundant links.

RSTP helps prevent switching loops by selecting appropriate forwarding paths and maintaining alternate paths for redundancy.

**Network Components:**
- Cisco Switches
- Ethernet Connections
- Redundant Network Links
- Cisco Packet Tracer

The complete network topology is available in the Packet Tracer project file.

## ⚙️ RSTP Configuration

### 1. Enable Rapid Spanning Tree Protocol

```bash
enable
configure terminal
spanning-tree mode rapid-pvst
end
```

### 2. Configure Root Bridge Priority

```bash
enable
configure terminal
spanning-tree vlan 1 priority 4096
end
```

The switch with the lowest Bridge ID becomes the Root Bridge.

### 3. Verify Spanning Tree Configuration

```bash
show spanning-tree
```

### 4. Verify VLAN 1 Spanning Tree

```bash
show spanning-tree vlan 1
```

### 5. Verify Root Bridge

```bash
show spanning-tree root
```

*Note: These are example commands for RSTP practice. The exact configuration should be checked in the Packet Tracer file.*

## 🔍 RSTP Port Roles

| Port Role | Description |
|---|---|
| Root Port | Provides the best path to the Root Bridge |
| Designated Port | Forwards traffic on a network segment |
| Alternate Port | Provides an alternative path to the Root Bridge |
| Backup Port | Provides backup connectivity on a shared segment |

## 🔄 RSTP Port States

RSTP uses three main port states:

| Port State | Description |
|---|---|
| Discarding | Prevents forwarding of user traffic |
| Learning | Learns MAC addresses |
| Forwarding | Forwards network traffic |

## ⚡ Difference Between STP and RSTP

| Feature | STP | RSTP |
|---|---|---|
| IEEE Standard | 802.1D | 802.1w |
| Convergence | Slower | Faster |
| Port States | 5 | 3 |
| Alternate Port | Not supported as a separate role | Supported |
| Network Recovery | Slower | Faster |

## 🧪 Network Verification

The following commands are useful for verifying RSTP configuration.

**Check Spanning Tree Status**

```bash
show spanning-tree
```

**Check Root Bridge Information**

```bash
show spanning-tree root
```

**Check RSTP Summary**

```bash
show spanning-tree summary
```

**Check VLAN 1 Spanning Tree**

```bash
show spanning-tree vlan 1
```

## 📚 Key Learnings

Through this lab, I focused on:

- Rapid Spanning Tree Protocol configuration.
- Root Bridge election using Bridge ID.
- Root Port and Designated Port selection.
- Alternate Port functionality.
- Layer 2 loop prevention.
- Redundant network connections.
- Faster network convergence.
- Cisco IOS configuration and verification.
- Basic network troubleshooting.

## 📁 Project File

`Rapitd STP.pkt`

Open the `.pkt` file using **Cisco Packet Tracer** to explore the network topology and configurations.

## 🚀 Skills Practiced

- Cisco Packet Tracer
- Rapid Spanning Tree Protocol (RSTP)
- Layer 2 Switching
- Root Bridge Election
- Bridge ID Comparison
- Network Redundancy
- Loop Prevention
- Network Convergence
- Cisco IOS CLI
- Network Troubleshooting

## 👨‍💻 CCNA Journey

This project is part of my ongoing **CCNA Journey** and hands-on networking practice.

Through practical networking labs, I am improving my understanding of switching technologies, network redundancy, and network troubleshooting.

**Learning Networking One Lab at a Time! 🌐🚀**
