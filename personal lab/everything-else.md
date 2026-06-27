# home lab

built to develop hands-on experience with enterprise networking, virtualization, identity,
and security monitoring.

## hardware

| Device | Role |
|--------|------|
| proxmox host | hypervisor — runs all VMs and LXC containers |
| fortigate 60D | firewall and router |
| cisco catalyst 3750X | core managed switch |
| aerohive AP230 | wireless access point |

## network topology

- 6 VLANs segmenting lab traffic by function
- fortigate handles inter-VLAN routing and firewall policy
- catalyst 3750X manages trunk and access port configuration

## virtualization

proxmox KVM hypervisor running the following workloads:

**security & monitoring**
- wazuh SIEM — log ingestion, alerting, and detection rules
- kali linux — security tooling practice and other excercises
- pi-hole — DNS-level ad and tracker blocking

**infrastructure**
- Ubuntu 22.04 LXCs — application workloads including bots

## skills demonstrated

- enterprise firewall policy and inter-VLAN routing
- managed switching, trunking, and VLAN segmentation
- hypervisor administration and VM lifecycle management
- SIEM deployment and detection engineering
- DNS management and network filtering
