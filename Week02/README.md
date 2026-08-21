# NexaCore Solutions – Enterprise Infrastructure Plan

## Project Overview
This project simulates the role of a Junior System Administrator tasked with designing the complete IT infrastructure for a newly established startup, **NexaCore Solutions**. The plan covers company profiling, hardware and software inventories, network design, IT role research, and infrastructure recommendations — built entirely from scratch for a 20-employee company with no existing computers, servers, network, or security policies.

## Learning Objectives
- Explain the roles and responsibilities of a System Administrator
- Identify hardware, software, and networking requirements for a small business
- Design an enterprise network topology
- Create professional technical documentation using Markdown
- Present infrastructure planning in a professional format

## Company Scenario
NexaCore Solutions is a 20-employee software development startup with four departments: IT (5), HR (4), Finance (5), and Sales (6). The company has no existing IT infrastructure — this project designs it from the ground up, from hardware procurement to network topology to security policy.

## Hardware Inventory Summary
- 12 desktop computers, 8 laptops, 1 server, routers/switches, printers, UPS units, wireless access points, NAS storage, and backup drives — sized to the 20-person headcount across all four departments.
- Full specifications and justifications are in `EnterpriseInfrastructurePlan.pdf`.

## Software Inventory Summary
- Windows 11 Pro and Ubuntu Server as base operating systems
- Microsoft 365 for productivity
- VS Code, Git, GitHub Desktop, and VirtualBox for the development team
- Microsoft Defender for endpoint security, AnyDesk for remote support

## Network Diagram
 <img width="1081" height="721" alt="Image" src="https://github.com/user-attachments/assets/5fe1a991-e5d1-41ee-a83f-84965ddd3cea" />

The topology flows from Internet → ISP Modem → Router → Firewall → Core Switch, branching out to the Wireless Access Point, Server, Printer, and all four department networks (Sales connects via Wi-Fi).

## Technologies Used
- Draw.io – network topology diagram
- Markdown – documentation
- Microsoft Word – formal infrastructure plan report
- GitHub – version control and portfolio hosting

## Challenges Encountered
Designing a network topology that was both technically accurate and easy to read was the most challenging part of this project — balancing proper networking symbols with a clean, logical layout took several iterations.

## Reflection
See the **Personal Reflection** section (Part 8) in `EnterpriseInfrastructurePlan.pdf` for a full discussion of what I learned and how this project prepared me for real-world system administration work.

## References
- LSPU Self-Paced Learning Module: System Administration and Maintenance
- Draw.io Documentation – https://www.drawio.com/doc/
- CompTIA Certification Guides – https://www.comptia.org/
