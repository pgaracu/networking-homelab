# Pablo's Homelab

Hi, I'm Pablo. 

This repository is designed to build and implement a quiet, power-aware networking lab that replicates the core functions of an enterprise network at home for networking and IoT/embedded-systems experiments, as well as serving as a sandbox to bring to life and test studied concepts that pertain to entry-level network certifications (CCNA, JNCIA-Junos). This setup will support practical work in Layer 1–3 networking, wireless segmentation, optical links, monitoring, automation, network-attached storage, and embedded endpoints.

The lab will have two operational areas:

1. An always-on infrastructure plane for internet access, monitoring,
   wireless service, storage, and power management.
2. An on-demand experimental plane that can be safely rebuilt, disrupted,
   and powered down when not in use.

Questions and recommendations are always welcome!

# Goals

The primary goal is to learn and have fun, and second: 

- Practice enterprise VLAN, trunking, routing, and firewall designs.
- Build multiple wireless networks mapped to security zones.
- Configure and troubleshoot copper and optical links.
- Simulate users, servers, and embedded devices with Raspberry Pis.
- Collect logs, metrics, traffic, and power-consumption data.
- Automate configuration validation and safe power management.
- Prepare for CCNA and JNCIA-Junos and future network engineering work.
- Develop a fundamental knowledge base in infrastructure automation,
  optical networking, wireless, or edge networking.

# Design principles

I designed this homelab keeping in mind equipment loudness, power efficiency, and power management. I envision a homelab that is:

- Quiet enough to operate in a bedroom.
- Low power when idle.
- Standards-based and vendor-diverse.
- Safe and enables separation between home and experimental networks.
- Locally manageable without requiring cloud services where practical.
- Reproducible through diagrams, configurations, and lab reports.

# Proposed architecture

![Logical network diagram](diagrams/exported/logical.svg)

![Power architecture](diagrams/exported/power.svg)

# Planned experiments

The following experiments cover the topics listed above:

1. VLAN and trunk configuration
2. Inter-VLAN routing and firewall policy
3. OSPF routing between simulated enterprise sites
4. Wireless SSID-to-VLAN mapping
5. Copper and optical link comparison
6. Network monitoring and alerting
7. Automated configuration backup and validation
8. Safe shutdown and startup through UPS and smart-PDU integration
9. Failure injection and recovery measurement

# Project status

- [x] Define project goals
- [x] Draft logical architecture
- [ ] Finalize exact bill of materials
- [ ] Acquire equipment
- [ ] Build the always-on infrastructure plane
- [ ] Build the experimental plane
- [ ] Complete the first five experiments
- [ ] Publish measurements and lessons learned
- [ ] Complete CCNA and/or JNCIA-Junos 

# Documentation

- [Architecture](docs/architecture.md)
- [Addressing and VLAN plan](docs/addressing-and-vlans.md)
- [Power design](docs/power-design.md)
- [Security model](docs/security-model.md)
- [Bill of materials](budget/bill-of-materials.md)
- [Learning roadmap](docs/learning-roadmap.md)

# Current stage

This repository currently represents the proposed design. Planned
configurations and expected outcomes will be replaced or supplemented by
tested results as equipment becomes available.
