Route Redistribution Lab – EVE-NG
This repository contains the EVE-NG topology, configuration files, and assets for the "Route Redistribution" practical lab. The lab demonstrates route redistribution between OSPF and EIGRP in a simulated network environment.

Lab Topology
R1: OSPF domain router

R2: Redistribution router (between OSPF and EIGRP)

R3: EIGRP domain router

The setup includes multiple ethernet links and switches, replicating a real-world scenario for route redistribution tasks.

![Lab Topology]
https://raw.githubusercontent.com/Ntwork-Beginner/EVE-NG/refs/heads/main/1st%20Practical%20Route%20Redistribution/Screenshot%202025-07-31%20150600.png

Router	Interface	IP Address	Connected To	Protocol
R1	Gi0/0	192.168.1.2/30	R2 Gi0/0	OSPF
R1	Gi0/1 / Gi0/2	172.20.20.1/24
172.20.10.1/24	Switch/SW	OSPF
R2	Gi0/0	192.168.1.1/30	R1 Gi0/0	OSPF
R2	Gi0/1	172.16.1.1/30	R3 Gi0/0	EIGRP
R3	Gi0/0	172.16.1.2/30	R2 Gi0/1	EIGRP
R3	Gi0/1 / Gi0/2	172.10.10.1/24
172.10.20.1/24	Switch/SW	EIGRP
Objectives
Understand and configure route redistribution between OSPF and EIGRP.

Analyze routing table changes after redistribution.

Test end-to-end connectivity across domains.

Instructions
Launch the EVE-NG topology file provided (.unl) in your EVE-NG environment.

Load the initial config files for R1, R2, and R3 (if included).

Follow the steps in the lab guide (Manual or Instructions folder, if present) to:

Set up OSPF routing on R1

Set up EIGRP routing on R3

Configure route redistribution on R2

Screenshots
See the /screenshots folder for sample run outputs and the recreated network topology.

Notes
All configurations use Cisco IOS images (replace as necessary for your setup).

The lab demonstrates basic redistribution—customize route-maps and filters for advanced use-cases.

Feel free to expand this README with step-by-step commands, troubleshooting tips, or add a section for common issues and solutions as your project evolves!
