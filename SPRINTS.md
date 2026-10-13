# Sprint plan

Eighteen sprints: three Foundations sprints (F1 to F3) for people new to IT, the fourteen core sprints (S0 through S13), and one Cisco networking sprint (N1) for Track G. Each teaches one skill area end to end, then ends with a "prove it" deliverable that someone else can check.

**Pacing assumption:** about 8 hours per week (3 reading or video, 4 hands-on lab, 1 review). Change the pace and the calendar moves, but not the order. Week counts below are planning estimates.

**Windows-first ordering:** S1 to S8 lean Windows and Azure so the AZ-802 gate lands first, about 5.8 months after S0. Each of those sprints has a short **Linux lane** to build the Linux skills in parallel.

Every lab in this file assumes the layout in [LAB-ENVIRONMENT.md](LAB-ENVIRONMENT.md).

**Foundations (Tracks F and E)**

| Sprint | Skill area | Weeks | Running total |
| --- | --- | --- | --- |
| F1 | Hardware, devices and troubleshooting | 3 | 3 |
| F2 | Networking fundamentals | 4 | 7 |
| **Gate** | **A+ Core 1** (1 review week) | 1 | 8 |
| F3 | Operating systems, security and support | 3 | 11 |
| **Gate** | **A+ Core 2** (1 review week) | 1 | 12 |
| **Gate** | **Network+** (2 review weeks) | 2 | 14 |

**Networking (Track G)**

| Step | Skill area | Weeks | Running total |
| --- | --- | --- | --- |
| F2 | Networking fundamentals | 4 | 4 |
| S0 | Lab and foundations | 2 | 6 |
| S1 | Networking and name resolution | 3 | 9 |
| N1 | Cisco routing and switching | 4 | 13 |
| **Gate** | **CCNA** (2 review weeks) | 2 | 15 |

**Core path (S0 to S13)**

| Sprint | Skill area | Weeks | Running total |
| --- | --- | --- | --- |
| S0 | Lab and foundations | 2 | 2 |
| S1 | Networking and name resolution | 3 | 5 |
| S2 | Identity and directory services | 4 | 9 |
| S3 | Hybrid identity and governance | 3 | 12 |
| S4 | Compute and virtualization | 3 | 15 |
| S5 | Storage and file services | 3 | 18 |
| S6 | Security and hardening | 3 | 21 |
| S7 | Monitoring, backup, troubleshooting | 3 | 24 |
| **Gate** | **AZ-802** (1 review week) | 1 | 25 |
| S8 | Automation and infrastructure as code | 3 | 28 |
| **Gate** | **AZ-104** (1 review week) | 1 | 29 |
| S9 | Cloud architecture and operations | 3 | 32 |
| **Gate** | **Cloud+ exam** (1 review week) | 1 | 33 |
| S10 | Linux services and advanced admin | 4 | 37 |
| **Gate** | **Linux+ and LPIC-1** (2 review weeks) | 2 | 39 |
| S11 | Security operations, governance, risk | 3 | 42 |
| **Gate** | **Security+** (1 review week) | 1 | 43 |
| S12 | Containers, virtualization, HA | 4 | 47 |
| **Gate** | **LPIC-2** (2 review weeks) | 2 | 49 |
| S13 | Capstone | 3 | 52 |
| **Gate** | **LPIC-3, one specialty** (2 review weeks) | 2 | 54 |

The core path is 54 weeks, about 12.5 months at 8 hours per week. Track E adds the 14 Foundations weeks in front, for 68 weeks (about 15.7 months). The earlier cert-by-cert roadmap came out near 18 months, so the overlap saves several months. Skip the gates for people on the skills-only track (see [TRACKS.md](TRACKS.md)).

**First exam timing:** counted from S0, AZ-802 lands at week 25 (about 5.8 months) at 8 hours per week. At 12 hours per week it lands around week 17 (about 4 months). On Track F and E the first exam is A+ Core 1, at week 8.

**Security+ timing:** V8 (SY0-801) launches on November 17, 2026, and V7 retires on June 11, 2027. Security+ comes at week 43 of the core sprints, so anyone starting after mid-2026 reaches it after V8 launches. Study the V8 objectives.

---

## Foundations (Track F, and the start of Track E)

Three sprints for people new to IT. They cover the hardware, operating system, support and networking basics that S0 to S13 assume, and lead to CompTIA A+ (two exams) and Network+. If you already work in IT support, or you can pass a Network+ practice exam, skip to S0.

**Why this order:** A+ Core 1 is about a quarter networking, so the networking sprint (F2) comes before the Core 1 exam. Network+ goes last, after F3 adds the security basics it also tests.

**Foundations lab:** the lab host from LAB-ENVIRONMENT.md, an old PC or laptop you can open up (a used office desktop is fine), a USB stick for installers, and your home router. Cisco Packet Tracer and Wireshark are free. F1 installs VMware Workstation and one Windows 11 VM, which becomes CL1 in S0.

## F1. Hardware, devices and troubleshooting (3 weeks)

**Outcome:** you can identify, install and troubleshoot PC, laptop, mobile and printer hardware, and you work every problem with the same troubleshooting method.

**Skills:** the CompTIA troubleshooting method, motherboards, CPUs, RAM, storage, power supplies, BIOS/UEFI and the boot process, display and peripheral connectors, laptops and mobile devices, printers, virtualization and cloud concepts.

**Labs**
1. Take apart the spare PC, identify every component, put it back together and boot it. Record each part's specs and connector types.
2. In UEFI, change the boot order, turn virtualization support (VT-x or AMD-V) and Secure Boot on and off, and set then clear a firmware password.
3. Add or swap RAM or a drive, then confirm the change in the operating system and in Disk Management.
4. Install VMware Workstation on the lab host and a Windows 11 VM. Snapshot it as `clean-install`.
5. Pair a phone with a laptop over Bluetooth, share the phone's hotspot, and add an email account to the phone. Note what each setting does.
6. Fault practice: a partner breaks one thing on the spare PC (pulls a RAM stick, unplugs a drive, changes the boot order). Find it using the six steps of the method.

**Prove it:** a hardware inventory of the spare PC, plus three troubleshooting tickets (symptom, theory, test, fix, check, notes) written in the order of the CompTIA method.

**Certs:** A+ Core 1 (hardware 25%, hardware and network troubleshooting 28%, mobile devices 13%, virtualization and cloud computing 11%).

## F2. Networking fundamentals (4 weeks)

**Outcome:** you can explain how data moves across a network, build a small switched and routed network, and troubleshoot it from the cable up to the application.

**Skills:** OSI and TCP/IP models, cabling and connectors, Ethernet switching and VLANs, IPv4 and IPv6 addressing and subnetting, routing basics, Wi-Fi standards and security, common ports and protocols, DHCP and DNS basics, NAT and VPN concepts, SNMP and syslog, network troubleshooting tools.

**Labs**
1. Install Cisco Packet Tracer (free with a Cisco Networking Academy account). Build two VLANs on one switch, route between them with a router, and give both VLANs DHCP.
2. Subnetting drill: split a /24 for four departments of different sizes. Check your answers with a calculator only after you finish.
3. Install Wireshark. Capture and label a DHCP exchange, a DNS lookup, a TCP three-way handshake and the start of an HTTPS connection.
4. Read your home router's settings: DHCP range, DNS servers, Wi-Fi band and security mode, port forwarding. Screenshot first and change nothing you can't put back.
5. Run the command-line tools on Windows and Linux: `ipconfig` and `ip`, `ping`, `tracert` and `traceroute`, `nslookup` and `dig`, `netstat` and `ss`, `arp`.
6. Fault practice in Packet Tracer: a partner breaks one thing (wrong VLAN, wrong gateway, a shut interface, a duplicate IP). Find and fix it.

**Prove it:** the Packet Tracer file with a diagram and addressing table, an annotated Wireshark capture, and a write-up of the fault practice.

**Certs:** Network+ (all five domains: concepts 23%, implementation 20%, operations 19%, security 14%, troubleshooting 24%) and A+ Core 1 networking (23%). S1 builds on this in the full lab.

**Gate: A+ Core 1 (220-1201)** happens here, with one review week.

## F3. Operating systems, security and support (3 weeks)

**Outcome:** you can install, configure and support Windows, find your way around macOS and Linux desktops, remove malware, and take a support ticket from first report to close.

**Skills:** Windows editions and installation, Settings and Control Panel, Task Manager, Event Viewer, Device Manager, Disk Management, Safe Mode and recovery, command prompt and PowerShell basics, users, groups, NTFS and share permissions, macOS and Linux desktop basics, physical and logical security, malware removal, data destruction, scripting basics, remote access tools, ticketing, change management, backups, safety and professionalism.

**Labs**
1. In the Windows 11 VM, create a standard user and an admin user, share a folder with different NTFS and share permissions, and test access as each user.
2. Work the tools: find a stopped service in Event Viewer, a missing driver in Device Manager, shrink a volume and add a partition in Disk Management, and boot into Safe Mode and the recovery options.
3. Install an Ubuntu desktop VM and do the same user and permission tasks from the terminal. Note the differences.
4. Malware removal: take a snapshot, trigger Microsoft Defender with the harmless EICAR test file, and follow CompTIA's malware removal steps in order, writing each one down. Revert the snapshot.
5. Backups: set up File History, delete a file and restore it.
6. Support practice: a partner sends three user tickets (can't print, slow PC, can't reach a share). Work each one in a ticket log, including the message you'd send the user.

**Prove it:** the ticket log, a permissions test table (user, folder, expected, actual) and the malware removal write-up.

**Certs:** A+ Core 2 (operating systems 28%, security 28%, software troubleshooting 23%, operational procedures 21%) and Network+ security (14%).

**Gate: A+ Core 2 (220-1202)** happens here, with one review week.

**Gate: Network+ (N10-009)** follows, with two review weeks: redo the F2 labs from memory, then practice exams.

---

## S0. Lab and foundations (2 weeks)

**Outcome:** a working, snapshotted lab, and comfort with the command line on both operating systems.

**Skills:** VMware Workstation networking, snapshots, Git basics, PowerShell and Bash basics, Linux filesystem layout, package management, reading logs.

**Labs**
1. Build the virtual networks and the router VM from LAB-ENVIRONMENT.md.
2. Install Windows Server, a Debian-family VM and a RHEL-family VM. Snapshot each as `clean-install`.
3. Copy this kit into your own Git repo, commit a change to your own progress file, and push.
4. Linux lane: navigate the filesystem, use `apt` and `dnf`, edit with `nano` and `vim`, read `journalctl` output.

**Prove it:** screenshot of all VMs running with correct IPs, plus a first commit in your progress file.

**Certs:** foundation for everything. LPIC-1 topics: system architecture, installation and package management, GNU and Unix commands.

## S1. Networking and name resolution (3 weeks)

**Outcome:** you can design and troubleshoot addressing, DNS and DHCP on both platforms.

**Skills:** IPv4 subnetting, routing, NAT, DNS zones and records, DHCP scopes and relay, hybrid name resolution concepts, firewall basics.

**Labs**
1. Configure the Linux router VM to route between the corp and branch networks with NAT to the internet.
2. Install DNS and DHCP on SRV1. Create forward and reverse zones. Add a DHCP scope with reservations.
3. Configure DHCP relay across the router to serve the branch network.
4. Set up a conditional forwarder and test it with `nslookup` and `Resolve-DnsName`.
5. Linux lane: configure static addressing with NetworkManager or netplan, run `bind9` or `dnsmasq` as a second resolver, capture traffic with `tcpdump`.

**Prove it:** a network diagram, and a one-page runbook showing how you diagnosed three deliberately broken settings (wrong gateway, wrong DNS, missing route).

**Certs:** AZ-802 (on-premises and hybrid networking), AZ-104 (virtual networking concepts), LPIC-1 (networking fundamentals), LPIC-2 (networking configuration).

## S2. Identity and directory services (4 weeks)

**Outcome:** you can build and run an Active Directory environment and apply policy at scale.

**Skills:** AD DS deployment, sites and replication, multi-domain concepts, users, groups, OUs, delegation, Group Policy, Linux users, groups and PAM basics.

**Labs**
1. Promote DC1 to a new forest. Add DC2 in the branch site with its own AD site and subnet.
2. Create an OU structure, security groups and 20 users with a PowerShell script.
3. Write GPOs for password policy, drive mappings and software restrictions. Test with `gpresult`.
4. Join CL1 and SRV1 to the domain. Delegate password reset rights to a helpdesk group.
5. Break replication on purpose and repair it with `repadmin` and `dcdiag`.
6. Linux lane: manage users and groups, configure `sudo` rules, explore PAM files, join LNX1 to the domain with `realmd` and `sssd`.

**Prove it:** the OU and GPO design document, the user creation script, and a recorded repair of the replication failure.

**Certs:** AZ-802 (AD DS is the largest domain, 20-25%), AZ-104 (identity concepts), Linux+ (user management), LPIC-1 (administrative tasks).

## S3. Hybrid identity and governance (3 weeks)

**Outcome:** you can connect on-premises identity to the cloud and control access and cost there.

**Skills:** Microsoft Entra ID, hybrid identity sync, role-based access control, Azure Policy, management groups, resource locks, tagging, Azure Arc, Azure budgets.

**Labs**
1. Set up an Azure free account with a budget alert before anything else.
2. Add a custom domain to Entra ID. Add a matching UPN suffix on-premises (a subdomain of a domain you own works).
3. Sync a subset of users with Entra Connect.
4. Create groups, assign built-in and custom Azure roles, and test them with a restricted user.
5. Apply an Azure Policy that requires a tag. Prove it blocks a non-compliant resource.
6. Onboard SRV1 to Azure Arc.

**Prove it:** an access matrix showing who can do what and why, and screenshots of the policy denying a deployment.

**Certs:** AZ-104 (identity and governance, 20-25%), AZ-802 (hybrid management), Cloud+ (IAM concepts).

## S4. Compute and virtualization (3 weeks)

**Outcome:** you can deploy and manage servers on-premises and in Azure and explain the tradeoffs.

**Skills:** Windows Server VMs, Azure VMs, images, scale and availability concepts, Linux virtualization basics (KVM, libvirt), container fundamentals.

**Labs**
1. Deploy a Windows Server VM and a Linux VM in Azure. Choose sizes, disks and network settings and justify each one.
2. Use custom script extensions to configure both VMs after deployment.
3. Compare an on-premises VMware VM and an Azure VM: backup, resize, move.
4. Deploy a container to Azure Container Instances or App Service and a second one on LNX1 with Docker or Podman.
5. Linux lane: install `libvirt` on LNX1 and inspect the VM definition files and virtual networks. Nested virtualization is off in this lab, so treat this as reading and light configuration, not running a second-level VM.

**Prove it:** a decision table for when to use a VM, a container, or an app service, with costs.

**Certs:** AZ-104 (compute, 20-25%), AZ-802 (Windows Server VMs in Azure), Cloud+ (deployment), Linux+ (containers), LPIC-3 305 (foundation).

## S5. Storage and file services (3 weeks)

**Outcome:** you can provide and protect storage for users and workloads on-premises and in Azure.

**Skills:** Windows file shares, permissions, DFS, Storage Spaces, Azure Files and Blob, access tiers, shared access signatures, Linux LVM, RAID, NFS and Samba.

**Labs**
1. Create file shares on SRV1 with NTFS and share permissions for three groups. Prove least privilege.
2. Set up DFS Namespaces across both sites and test failover.
3. Build a Storage Space with a resilient volume on added virtual disks.
4. Create an Azure storage account, an Azure Files share and a Blob container. Mount the file share on SRV1.
5. Generate a shared access signature and a stored access policy. Revoke access.
6. Linux lane: build LVM volumes, extend one live, configure software RAID and an NFS export.

**Prove it:** a permissions matrix and a test log showing users can and cannot reach each share.

**Certs:** AZ-802 (storage and file services, 15-20%), AZ-104 (storage, 15-20%), LPIC-1 (filesystems), LPIC-2 (advanced storage, file sharing), Linux+ (system management).

## S6. Security and hardening (3 weeks)

**Outcome:** you can measure a server against a baseline and fix the gaps.

**Skills:** OS hardening, patching, Windows Defender and firewall, secure AD, least privilege, Linux firewall and SELinux or AppArmor, TLS and certificates, vulnerability scanning.

**Labs**
1. Apply a security baseline to SRV1 with GPO and document the differences before and after.
2. Configure Windows Firewall rules through policy and test them.
3. Deploy an internal certificate authority. Issue a certificate and bind it to a web service.
4. Review AD for risky settings (stale accounts, weak delegation, legacy protocols) and remediate.
5. Run a vulnerability scan (OpenVAS or similar) against the lab and rank the findings.
6. Linux lane: configure `nftables` or `firewalld`, enforce SELinux on LNX2, set SSH key-only login on LNX1.

**Prove it:** a hardening report with before-and-after evidence for at least ten controls.

**Certs:** AZ-802 (secure Windows Server and AD DS), Cloud+ (security), Security+ (security architecture and controls), Linux+ (security, 18%), LPIC-2 (system security), LPIC-3 303 (foundation).

## S7. Monitoring, backup and troubleshooting (3 weeks)

**Outcome:** you can watch systems, restore them, and find faults methodically.

**Skills:** Performance Monitor, Event Viewer, Windows Admin Center, Azure Monitor, Log Analytics, alerts, backup and recovery, disaster recovery basics, a repeatable troubleshooting method, Linux logs and performance tools.

**Labs**
1. Collect performance counters from SRV1 and set an alert threshold.
2. Send logs from SRV1 to a Log Analytics workspace. Write two queries.
3. Back up SRV1 files and a system state. Delete data and restore it.
4. Configure Azure Backup for an Azure VM and test a restore.
5. Fault lab: a partner (or a script) breaks something in the lab. You diagnose and fix it using only logs and tools, and write up the timeline.
6. Linux lane: use `journalctl`, `top`, `iostat`, `ss`, and `systemd` status to diagnose a stuck service and a full disk.

**Prove it:** a monitoring dashboard screenshot, a restore test log, and an incident write-up with root cause.

**Certs:** AZ-802 (monitor and troubleshoot, 15-20%), AZ-104 (monitor and maintain, 10-15%), Linux+ (troubleshooting, 22%), Cloud+ (operations, troubleshooting).

**Gate: AZ-802.** See ASSESSMENT.md for readiness criteria.

## S8. Automation and infrastructure as code (3 weeks)

**Outcome:** you can build repeatable environments from code instead of by hand.

**Skills:** PowerShell scripting and modules, Bash scripting, ARM templates and Bicep, Azure CLI, Ansible basics, Git workflows, secrets handling.

**Labs**
1. Rewrite the S2 user creation script with parameters, logging and error handling.
2. Deploy a virtual network, a storage account and a VM from a Bicep file. Redeploy it to prove it is repeatable.
3. Write the same deployment with the Azure CLI and compare.
4. Write an Ansible playbook that configures LNX1 and LNX2 identically (users, packages, firewall, SSH).
5. Put every script into Git with meaningful commits and a README.
6. Linux lane: write a Bash script with functions, arguments and a cron or systemd timer.

**Prove it:** a repo folder of scripts and templates that a teammate can run cold to rebuild an environment.

**Certs:** AZ-104 (ARM and Bicep), Linux+ (automation, orchestration and scripting, 17%), Cloud+ (DevOps fundamentals), LPIC-1 (shell scripting).

**Gate: AZ-104.**

## S9. Cloud architecture and operations (3 weeks)

**Outcome:** you can pick the right cloud design and explain cost, risk and migration.

**Skills:** cloud service and deployment models, shared responsibility, high availability and disaster recovery design, cost management, migration approaches, multicloud concepts, cloud security and IAM patterns.

**Labs**
1. Design a three-tier application on paper, then price it in the Azure calculator in two regions.
2. Compare the same design on a second cloud using its published pricing (no deployment needed).
3. Write a migration plan for the lab file server to Azure Files with a rollback.
4. Review a sample architecture and mark single points of failure.
5. Set up cost alerts and tag-based cost reports in Azure.

**Prove it:** an architecture document with diagram, cost estimate, risks and migration plan.

**Certs:** Cloud+ (architecture 23%, deployment 19%, operations 17%), AZ-104 (reinforcement).

**Gate: Cloud+.** Check the exam's retirement date before booking. CompTIA lists an estimated 2027.

## S10. Linux services and advanced administration (4 weeks)

**Outcome:** you can run the core network services and manage boot, kernel and capacity on Linux.

**Skills:** DNS, web, mail and file-sharing services, boot process and systemd, kernel modules, capacity planning, system maintenance, networking configuration.

**Labs**
1. Run authoritative DNS with `bind9` for a lab zone and test from Windows.
2. Host two virtual sites with Apache or Nginx, TLS and a reverse proxy.
3. Set up a small mail relay with Postfix and test delivery.
4. Configure Samba to serve a share to a domain user.
5. Trace the boot process, break the bootloader on a snapshot and recover it.
6. Build a capacity report from `sar` or similar tools.

**Prove it:** a service catalogue for the lab (what runs, where, how to restore it) and boot recovery notes.

**Certs:** Linux+ (system management, services, troubleshooting), LPIC-1 (all topics reinforced), LPIC-2 (DNS, web, file sharing, email, kernel, startup, capacity planning).

**Gate: Linux+ and LPIC-1.** They overlap heavily, so plan them close together.

## S11. Security operations, governance and risk (3 weeks)

**Outcome:** you can detect and respond to incidents and explain security in business terms.

**Skills:** threats and vulnerabilities, log analysis, incident response, security tools, risk assessment, policy and compliance, data protection, security awareness.

**Labs**
1. Centralize logs from the lab into one place and write three detection rules.
2. Run a tabletop incident exercise from a written scenario. Document the timeline and lessons learned.
3. Write a risk register for the lab with likelihood, impact and controls.
4. Draft an acceptable use policy and a backup policy and map each to controls in the lab.
5. Simulate a phishing report and walk the response steps.

**Prove it:** the risk register, an incident report and three tested detection rules.

**Certs:** Security+ (security operations, threats and vulnerabilities, governance, risk and compliance). The V8 objectives add more AI risk, so review them when published.

**Gate: Security+.**

## S12. Containers, virtualization and high availability (4 weeks)

**Outcome:** you can run and secure containers and design for availability.

**Skills:** container images and runtimes, orchestration basics, virtualization platforms, clustering, load balancing, shared storage, failover, hardening containers.

**Labs**
1. Build a container image, publish to a private registry and run it with limits.
2. Run a three-container app with Compose or Podman pods.
3. Build a two-node web cluster with a shared IP and test failover.
4. Set up a load balancer in front of two web servers and pull one node offline.
5. Scan an image for vulnerabilities and fix the findings.

**Prove it:** a documented failover test with timings and a container hardening checklist.

**Certs:** LPIC-3 305 or 306 (choose a track now), Cloud+ (deployment, DevOps), Linux+ (containers).

**Gate: LPIC-2** happens here. LPIC-2 needs an active LPIC-1.

## S13. Capstone (3 weeks)

**Outcome:** one integrated environment that proves the whole skill set.

**Build:** a small company environment with two sites, a domain, hybrid identity, file services, a Linux service tier, monitoring, backup, hardening, and an automated rebuild.

**Requirements**
1. Everything defined in code where possible, stored in Git.
2. A documented architecture, runbook and recovery test.
3. A security review with findings fixed.
4. A 20-minute walkthrough to teammates.

**Prove it:** the walkthrough, judged against the rubric in ASSESSMENT.md.

**Gate: LPIC-3, one specialty.**

---

## Networking (Track G)

One Cisco sprint for people heading into network administration or a network operations center. It builds on F2 and S1 and leads to the CCNA.

**CCNA version:** this sprint follows CCNA v2.0, the only version from February 3, 2027. The exam code stays 200-301. Version 2.0 puts more weight on troubleshooting and adds AI in network operations. Check Cisco's v2.0 exam topics before you start. If your CCNA gate lands before February 3, 2027, either book v1.1 by February 2 or keep studying v2.0 and book after the switch. Don't split the difference.

**Cisco lab:** Cisco Packet Tracer (from F2) covers most labs. Cisco Modeling Labs Free (up to five nodes) runs real IOS images for the labs Packet Tracer can't do.

## N1. Cisco routing and switching (4 weeks)

**Outcome:** you can build, secure and troubleshoot a small Cisco campus network, and use automation and AI tools without trusting them blindly.

**Skills:** Cisco IOS configuration and show commands, VLANs and 802.1Q trunks, Rapid PVST+, EtherChannel, inter-VLAN routing, static routes, OSPFv2 and OSPFv3, HSRP, NAT and PAT, DHCP, NTP, syslog and SNMP on IOS, SSH and SCP, ACLs, port security, DHCP snooping, dynamic ARP inspection, storm control, wireless LAN controllers, REST APIs and JSON, AI-assisted network operations.

**Labs**
1. Campus switching: two switches with VLANs, a trunk, LACP EtherChannel and inter-VLAN routing on a layer-3 switch. Set the root bridge with Rapid PVST+, and add PortFast and BPDU guard on access ports.
2. Routing: three routers in single-area OSPFv2, then add IPv6 and OSPFv3. Add a floating static route as a backup path and test it.
3. Redundancy: run HSRP between two routers, shut one down and watch the failover.
4. Services: DHCP, NAT and PAT, NTP and syslog on IOS. Allow SSH only, with local users, and back up a config with SCP.
5. Security: standard and extended ACLs, port security, DHCP snooping, dynamic ARP inspection and storm control. Set up a WPA3 wireless network on a controller in Packet Tracer.
6. Automation and AI: in Cisco Modeling Labs Free, read a device's configuration as JSON through RESTCONF. Ask an AI assistant to draft the fix for one fault. Check every line against the device before you apply it, and note what it got wrong.
7. Fault practice: a partner breaks four things (native VLAN mismatch, OSPF area mismatch, ACL in the wrong order, HSRP priority). Find each one with show commands.

**Prove it:** the lab file with a diagram and addressing table, the device configs in Git, and a troubleshooting log for the four faults.

**Certs:** CCNA v2.0 (infrastructure and connectivity 25%, switching and network access 25%, IP routing 20%, network services and security 20%, AI and network operations 10%).

**Gate: CCNA (200-301)** happens here, with two review weeks.
