# 🗄️ 12U Homelab: The Bare-Metal Foundation

![Final 12U Rack Build](images/hero_shot_placeholder.png)
*Ideal Picture: A clean, well-lit "hero shot" of the fully assembled 10-inch 12U rack, powered on, with the locking glass door either closed or slightly open to show off the equipment LEDs.*

## 📅 1. Overview & The Four-Year Evolution
This project represents the culmination of my four years in the CIT Cybersecurity program, transitioning my infrastructure from a [custom 3D-printed TrueNAS appliance](https://github.com/esixtosr/3D-Printed-TRUENAS) into a scalable, enterprise-grade 12U server rack.

Over the course of my degree, my technical requirements drastically evolved, and this physical build reflects that journey:
*   **The Foundation (Years 1 & 2):** It started with basic system administration, spinning up standalone VMs, and grasping the fundamentals of subnetting, VLANs, and LDAP.
*   **The Escalation (Years 3 & 4):** The focus shifted from basic networking to managing segmented environments, implementing cloud control, and diving into penetration testing. Eventually, the requirements scaled up to advanced incident response, firewall administration, and VPN deployments.

I needed a physical environment capable of supporting all of those complex, senior-level requirements in one unified stack.

## 🗺️ 2. Project Goals & Physical Topology (Layer 1)
The primary goal of this physical build was to create the bare-metal backbone required to host a highly secure, segmented network. To keep the infrastructure manageable and easy to troubleshoot, the physical cabling follows a strict top-down hierarchy:

*[Insert Network Topology Diagram Here]*

![Network Topology Cabling](images/patch_panel_placeholder.png)
*Ideal Picture: A close-up shot focused specifically on your patch panel and core managed switch. Show off the clean, color-coded patch cables connecting your firewall, switch, and incoming data lines.*

*Note: The software configurations, virtual network topologies, and security deployments hosted on this physical hardware are documented separately.*
*   ↳ **[Link to Logical Architecture Repo/Folder]:** *Documentation covering the deployment of my Proxmox hypervisors, Active Directory domains, and segmented virtual environments.*

## 📋 3. Bill of Materials (Hardware & Infrastructure)
Below is the breakdown of the physical hardware, networking equipment, custom 3D prints, and power management utilized in this specialized 10-inch rack build.

![Hardware Unboxed](images/hardware_inventory_placeholder.png)
*Ideal Picture: A photo of your bare-metal servers, switch, and PDU laid out on a table or floor before racking them. Alternatively, a straight-on, eye-level shot of the front of the rack highlighting the neatly stacked components.*

| Category | Components | Purpose / Notes |
| :--- | :--- | :--- |
| **Enclosure & Power** | • [10-Inch 12U Server Rack](https://a.co/d/08EilrVu)<br>• [1U 10-Inch Rack Power Hub](https://a.co/d/0j3JPrRW)<br>• [M6 Cage Nuts & Screws](https://a.co/d/0iliX7vH) | The primary locking chassis, power distribution (PDU), and standardized mounting hardware. |
| **Core Networking** | • [UniFi Cloud Gateway Fiber](https://store.ui.com/us/en/category/cloud-gateways-compact/collections/cloud-gateway-fiber/products/ucg-fiber)<br>• [UniFi USW-Flex-2.5G 8-Port PoE Switch](https://store.ui.com/us/en/category/switching-utility/products/usw-flex-2-5g-8-poe)<br>• [UniFi U7 Pro AP](https://store.ui.com/us/en/category/wifi-flagship/products/u7-pro) | Handles the primary firewall routing, high-speed PoE edge switching, and wireless access points. |
| **Cable Management** | • [12-Port Cat6a Mini Patch Panel](https://a.co/d/09bkBMMH)<br>• [Cat6 0.5ft Cables](https://a.co/d/03gDXVx2)<br>• [Cat6 1ft Cables](https://a.co/d/00AY766S) | Distributes physical network connections cleanly across the front of the 10-inch standard rack. |
| **Compute Nodes** | • [Lenovo ThinkCentre M720q](https://a.co/d/0fbYrNjp)<br>• 2x [Raspberry Pi 5 (8GB)](https://a.co/d/0i0JTN0H)<br>• [SFF PC Keystones](https://a.co/d/0hwqE5ym) | Primary bare-metal compute nodes for hypervisors and lightweight auxiliary tasks. |
| **Storage Array** | • [Custom 3D-Printed TrueNAS Appliance](https://github.com/esixtosr/3D-Printed-TRUENAS)<br>• [4-Bay 2.5" SSD Caddies](https://a.co/d/0apoSDdO)<br>• [2-Bay 3.5" HDD Caddies](https://a.co/d/07yT3Vlt)<br>• [SATA to SATA Adapters](https://a.co/d/0h5rM0cd) | Centralized network storage utilizing custom drive caddies and adapters for density. |
| **Custom 3D Prints** | • [10-Inch 12U Rack Print Collection](https://makerworld.com/en/collections/28263383-10-inch-12u-mini-server-rack)<br>• [PETG Filament](https://a.co/d/0fkblDBF) | Custom-fabricated mounts, shelves, and brackets designed specifically for the 10-inch form factor. |
| **Accessories** | • [7.84-Inch 2U Rack Screen](https://a.co/d/0h06jV71)<br>• [Gorilla Mounting Tape](https://a.co/d/0biTWiEH) | Front-facing rack monitoring display and secure mounting for non-rackable components. |

## 🛠️ 4. The Build Process & Hardware Tips
Building out a 12U rack requires a different mindset than building a standard PC. Here are the tools I used and the trial-and-error lessons I learned regarding rack mounting and cable management:

![Work in Progress](images/cable_management_placeholder.png)
*Ideal Picture: A "behind-the-scenes" shot of the back of the rack showing your cable management strategy (zip ties/velcro strips), power cord routing, or a mid-build photo with your tools (screwdrivers, cage nuts, crimpers) scattered around.*

*   **Tools Required:** *Mention things like cage nut tools, specific screwdrivers, crimpers, or cable testers.*
*   **Cable Management Strategy:** *Talk about patch panel routing, color-coding data lines, separating power cables from data cables, and zip-tie/velcro usage.*
*   **Clearance & Thermals:** *Discuss any issues you had sliding rails in, managing heat exhaust with rack fans, or physical weight distribution (heaviest stuff at the bottom).*

## 🧠 5. Final Thoughts & Lessons Learned
*A summary of what it actually takes to plan, purchase, and assemble enterprise networking gear versus standard consumer hardware. Reflect on how having this dedicated physical space changes the way you approach virtualization and network security.*

---

## 🤝 6. Inspiration & Credits
This specific 10-inch mini-rack build was heavily inspired by some incredible creators in the homelab and 3D-printing community. A massive shoutout to the following resources that helped guide the physical architecture and custom fabrication of this project:

*   **Jeff Geerling:** For his pioneering work on [The Mini Rack Project](https://mini-rack.jeffgeerling.com) and his foundational [10-inch Raspberry Pi Rack build](https://youtu.be/y1GCIwLm3is?si=MwU9eaMKf_API1G3).
*   **Hardware Haven:** For the custom NAS enclosure concept and assembly guidance showcased in his [3D-Printed NAS build](https://youtu.be/776-6ph7zsQ?si=3X3mC2kIXBhyUZ9f).
*   **Techno Tim:** For invaluable enterprise homelab inspiration, specifically his [homelab rack tours](https://youtu.be/Ghuc1vfiLiM?si=-DRlllYZvw6woj-u) and [server architecture overviews](https://youtu.be/kGZa-81IDGY?si=inZfo1SUED2QK0Xl).
