# 🗄️ 12U Mini Server Rack Homelab

![Final 12U Rack Build](images/hero_shot_placeholder.png)

*A compact 10-inch 12U homelab rack built to support virtualization, segmented networking, storage, monitoring, and cybersecurity lab work.*

---

## 📌 Overview

This project documents the physical buildout of my 12U mini server rack homelab. The goal was to move from a loose collection of devices and a custom 3D-printed TrueNAS system into a cleaner, rack-mounted infrastructure stack that could support my cybersecurity, networking, and systems administration work.

The rack is designed around a compact 10-inch form factor while still supporting core homelab services such as:

- Virtualization
- Network segmentation
- Firewall and routing experiments
- Centralized storage
- Lightweight monitoring
- Raspberry Pi services
- Cybersecurity lab environments
- Custom 3D-printed rack mounts and accessories

This is the physical foundation for the larger lab environment I use for hands-on infrastructure, security, and networking projects.

---

## 🧭 Project Background

My homelab started as a smaller setup focused on basic system administration, virtual machines, and storage. Over time, my needs grew as I moved deeper into cybersecurity and network engineering.

Earlier stages of the lab focused on:

- Learning Linux and Windows Server administration
- Running standalone virtual machines
- Understanding subnetting, VLANs, and basic network services
- Building a custom 3D-printed TrueNAS appliance

As the lab evolved, I needed a more organized physical setup that could handle:

- Segmented networks
- Firewall rule testing
- VPN deployments
- Proxmox virtualization
- Active Directory labs
- NAS storage
- Raspberry Pi services
- Security monitoring and logging experiments

This rack build brings those pieces into one cleaner and more scalable physical environment.

---

## 🗺️ Physical Topology

The primary goal of this build was to create a compact but organized rack that could serve as the bare-metal backbone for my homelab.

To plan the layout, I also built a custom interactive network topology tool for mapping devices, physical ports, and rack connections.

![Interactive Network Topology Walkthrough](images/topology_walkthrough.gif)

**Live Topology Preview:**  
[Open the interactive network topology](network-topology.html)

> **Note:** The topology page is intended to show physical connections, port assignments, and device relationships. Logical services such as Proxmox, Active Directory, VLANs, and security tools may be documented separately.

---

## 📋 Bill of Materials

| Category | Components | Purpose |
| :--- | :--- | :--- |
| **Rack & Power** | [10-Inch 12U Server Rack](https://a.co/d/08EilrVu)<br>[1U 10-Inch Rack Power Hub](https://a.co/d/0j3JPrRW)<br>[M6 Cage Nuts & Screws](https://a.co/d/0iliX7vH) | Main rack enclosure, power distribution, and mounting hardware |
| **Core Networking** | [UniFi Cloud Gateway Fiber](https://store.ui.com/us/en/category/cloud-gateways-compact/collections/cloud-gateway-fiber/products/ucg-fiber)<br>[UniFi USW-Flex-2.5G 8-Port PoE Switch](https://store.ui.com/us/en/category/switching-utility/products/usw-flex-2-5g-8-poe)<br>[UniFi U7 Pro AP](https://store.ui.com/us/en/category/wifi-flagship/products/u7-pro) | Firewall, routing, switching, PoE, and wireless connectivity |
| **Cable Management** | [12-Port Cat6a Mini Patch Panel](https://a.co/d/09bkBMMH)<br>[Cat6 0.5ft Cables](https://a.co/d/03gDXVx2)<br>[Cat6 1ft Cables](https://a.co/d/00AY766S) | Clean front-facing network patching and short cable runs |
| **Compute** | [Lenovo ThinkCentre M720q](https://a.co/d/0fbYrNjp)<br>2x [Raspberry Pi 5 8GB](https://a.co/d/0i0JTN0H)<br>[SFF PC Keystones](https://a.co/d/0hwqE5ym) | Main compute node and lightweight auxiliary services |
| **Storage** | [Custom 3D-Printed TrueNAS Appliance](https://github.com/esixtosr/3D-Printed-TRUENAS)<br>[4-Bay 2.5-inch SSD Caddies](https://a.co/d/0apoSDdO)<br>[2-Bay 3.5-inch HDD Caddies](https://a.co/d/07yT3Vlt)<br>[SATA to SATA Adapters](https://a.co/d/0h5rM0cd) | Centralized network storage and custom drive mounting |
| **3D Prints** | [10-Inch 12U Rack Print Collection](https://makerworld.com/en/collections/28263383-10-inch-12u-mini-server-rack)<br>[PETG Filament](https://a.co/d/0fkblDBF) | Custom shelves, brackets, mounts, and rack accessories |
| **Accessories** | [7.84-Inch 2U Rack Screen](https://a.co/d/0h06jV71)<br>[Gorilla Mounting Tape](https://a.co/d/0biTWiEH) | Rack display and mounting support for non-rackable components |

---

## 🛠️ Build Notes

Building in a compact 10-inch rack forced me to pay close attention to spacing, airflow, cable length, and mounting options. Unlike a full-size rack, there is very little room to hide messy cabling or oversized hardware.

### 3D Printing

Most custom brackets and shelves were printed in PETG instead of PLA. PETG is better suited for this type of setup because it handles heat and long-term stress better than standard PLA.

This was especially important for parts mounted near:

- The Lenovo compute node
- UniFi networking equipment
- Power distribution hardware
- Drive caddies
- Enclosed rack airflow paths

### Cable Management

Short patch cables were used wherever possible to avoid large cable loops inside the rack. The front patch panel keeps connections cleaner and makes it easier to trace physical links between devices.

The goal was not just to make the rack look clean, but to make troubleshooting easier later.

### Weight and Layout

Heavier components were placed lower in the rack to keep the center of gravity stable. Power distribution and storage components sit toward the bottom, while lighter devices such as Raspberry Pis, patch panels, and accessories are mounted higher.

### Compact Rack Challenges

The biggest challenge with this build was making consumer, prosumer, and custom hardware work inside a small 10-inch rack standard. Some parts fit cleanly, while others required custom mounts, adapters, or creative spacing.

This build required a mix of:

- Rack hardware
- 3D-printed parts
- Keystone adapters
- Short patch cables
- Careful cable routing
- Trial and error

Tiny rack, big attitude.

---

## 🧠 Lessons Learned

This project taught me that the physical side of infrastructure matters just as much as the software side. A clean rack makes future projects easier because power, networking, storage, and compute are already organized.

Some of the biggest takeaways were:

- Plan physical layout before buying parts.
- Leave more room for cables than expected.
- Short cables help, but only if the patching layout makes sense.
- PETG is worth using for functional rack parts.
- A compact rack looks clean, but it leaves very little margin for bad planning.
- Good documentation makes the lab easier to rebuild, troubleshoot, or explain later.

This rack is not meant to be a data center. It is a practical, small-scale infrastructure lab that lets me test real networking, storage, virtualization, and cybersecurity concepts in a controlled environment.

---

## 🔗 Related Projects

- [3D-Printed TrueNAS Appliance](https://github.com/esixtosr/3D-Printed-TRUENAS)
- Interactive Network Topology: `network-topology.html`
- Logical Infrastructure Documentation: Coming soon

---

## 🤝 Inspiration & Credits

This build was inspired by several creators in the homelab and 3D-printing community:

- **Jeff Geerling** — For his work on [The Mini Rack Project](https://mini-rack.jeffgeerling.com) and his 10-inch Raspberry Pi rack builds.
- **Hardware Haven** — For inspiration around compact, custom NAS builds and 3D-printed storage systems.
- **Techno Tim** — For homelab infrastructure, rack organization, and practical self-hosting inspiration.

Their work helped shape the direction of this build, especially around compact rack design, 3D-printed mounting, and clean homelab documentation.
