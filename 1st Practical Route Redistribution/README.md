Route Redistribution Lab – EVE-NG
This repository contains the EVE-NG topology, configuration files, and assets for the "Route Redistribution" practical lab. The lab demonstrates route redistribution between OSPF and EIGRP in a simulated network environment.

Lab Topology
R1: OSPF domain router

R2: Redistribution router (between OSPF and EIGRP)

R3: EIGRP domain router

The setup includes multiple ethernet links and switches, replicating a real-world scenario for route redistribution tasks.

![Lab Topology]



<img width="1180" height="633" alt="Screenshot 2025-07-31 150600" src="https://github.com/user-attachments/assets/a8427c14-2bb4-41bb-b1c2-29e3a2d3ccd4" />


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
