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
Below is the breakdown of the physical hardware, networking equipment, and power management utilized in this 12U build.

![Hardware Unboxed](images/hardware_inventory_placeholder.png)
*Ideal Picture: A photo of your bare-metal servers, switch, and PDU laid out on a table or floor before racking them. Alternatively, a straight-on, eye-level shot of the front of the rack highlighting the neatly stacked components.*

| Category | Item | Purpose / Notes |
| :--- | :--- | :--- |
| **Enclosure** | 10-inch 12U Server Rack | The primary chassis featuring a locking front door. |
| **Networking** | [Insert Switch] | Core switching for physical VLAN segmentation. |
| **Compute** | [Insert Server/Hosts] | Primary bare-metal compute nodes running Proxmox. |
| **Storage** | [Insert TrueNAS/SAN] | Centralized storage array. |
| **Power** | [Insert PDU / UPS] | Power distribution and battery backup for graceful shutdowns. |

## 🛠️ 4. The Build Process & Hardware Tips
Building out a 12U rack requires a different mindset than building a standard PC. Here are the tools I used and the trial-and-error lessons I learned regarding rack mounting and cable management:

![Work in Progress](images/cable_management_placeholder.png)
*Ideal Picture: A "behind-the-scenes" shot of the back of the rack showing your cable management strategy (zip ties/velcro strips), power cord routing, or a mid-build photo with your tools (screwdrivers, cage nuts, crimpers) scattered around.*

*   **Tools Required:** *Mention things like cage nut tools, specific screwdrivers, crimpers, or cable testers.*
*   **Cable Management Strategy:** *Talk about patch panel routing, color-coding data lines, separating power cables from data cables, and zip-tie/velcro usage.*
*   **Clearance & Thermals:** *Discuss any issues you had sliding rails in, managing heat exhaust with rack fans, or physical weight distribution (heaviest stuff at the bottom).*

## 🧠 5. Final Thoughts & Lessons Learned
*A summary of what it actually takes to plan, purchase, and assemble enterprise networking gear versus standard consumer hardware. Reflect on how having this dedicated physical space changes the way you approach virtualization and network security.*
