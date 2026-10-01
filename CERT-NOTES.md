# Certification notes

> **Note:** The order of study in this file was the first draft, organized by certification. The current plan is skills-first and lives in [SPRINTS.md](SPRINTS.md). Use this file for the exam facts and sources only.

Last checked: 2026-09-29. Exam versions and retirement dates change, so re-check the official pages before booking any exam.

## Assumptions (change these and the dates move)

- About 8 hours per week: roughly 3 hours reading or video, 4 hours hands-on lab, 1 hour practice questions.
- First exam (AZ-802) about 3 to 4 months from now, within your 3 to 6 month target.
- Lab host: Core 7 150U, 32GB RAM, 1TB NVMe, VMware Workstation. Nested Hyper-V is out of scope for this lab.
- Hours per cert are rough planning numbers, not Microsoft, CompTIA or LPI figures.

## The certifications

| Cert | Exam(s) | Format | Notes |
| --- | --- | --- | --- |
| Microsoft AZ-802, Administering Windows Server | AZ-802 | Pass mark 700 | AD DS 20-25%, storage 15-20%, monitor/troubleshoot 15-20%, hybrid mgmt, VMs, networking, security 10-15% each |
| Microsoft AZ-104, Azure Administrator | AZ-104 | Pass mark 700 | Identity/governance 20-25%, compute 20-25%, storage 15-20%, networking 15-20%, monitor/backup 10-15% |
| CompTIA Cloud+ | CV0-004 | 90 min, max 90 questions, pass 750 | Released Sep 2024. CompTIA lists an estimated 2027 retirement, so do it earlier |
| CompTIA Security+ | SY0-701 (V7) now, V8 expected around Nov 17, 2026 | see note | V8 adds more AI risk, security operations, modern environments. Third-party sources report the V8 code as SY0-801. Confirm on comptia.org |
| CompTIA Linux+ | XK0-006 | 90 min, max 90 questions, pass 720 | Released Jul 2025. Estimated 2028 retirement |
| LPIC-1 | 101-500, 102-500 | 90 min, 60 questions each | No prerequisite. Valid 5 years |
| LPIC-2 | 201-450, 202-450 | 90 min, 60 questions each | Requires an active LPIC-1 |
| LPIC-3 | 300, 303, 305 or 306 | One track of four | Pick one track. Check prerequisites on lpi.org |

Note: some older study plans mention LPIC 1-4. LPI has no LPIC-4. LPIC-3 has four tracks: Mixed Environments (300), Security (303), Virtualization and Containerization (305), High Availability and Storage Clusters (306). 303 and 305 fit best with the rest of this plan.

## Order and why

1. **AZ-802** (months 1-4). Most lab-heavy. Builds the base lab that later certs reuse.
2. **AZ-104** (months 4-7). Shares Entra ID, Azure Files, VMs, storage and monitoring with AZ-802, so it moves faster after it.
3. **Cloud+ CV0-004** (months 7-8). Best overlap with AZ-104 while it's fresh, and the exam is expected to retire in 2027.
4. **Security+** (months 9-10). See the decision below.
5. **Linux+ XK0-006** (months 11-12).
6. **LPIC-1** (months 13-14). Large overlap with Linux+, so it should be a short step.
7. **LPIC-2** (months 15-18). Needs an active LPIC-1.
8. **LPIC-3**, one track (month 19 onward).

That is roughly a year and a half of study at 8 hours per week. If you want it shorter, drop LPIC-2 and LPIC-3 first, since Linux+ and LPIC-1 cover the same ground for most jobs.

## Decision: Security+ V7 or V8

V8 is due about seven weeks from today. In this plan you'd study during the V8 window, so aim for V8 and skip V7. If you need the cert sooner for work, take V7 as a separate sprint before the V8 launch, but that would delay AZ-802.

## Overlap map

- **AZ-802 and AZ-104:** Entra ID, Azure Files, Azure VMs, storage, monitoring, backup.
- **AZ-104 and Cloud+:** cloud concepts, networking, storage, deployment, security.
- **Cloud+ and Security+:** cloud security, IAM, logging and monitoring.
- **Linux+ and LPIC-1:** shell, packages, filesystems, users, services, networking, scripting.
- **LPIC-2 and LPIC-3:** services, networking and security depth on Linux.

## Lab plan (32GB host)

Run only what the current study block needs. Suspend the rest and take snapshots before every change.

**AZ-802 block (about 12-14GB at a time):**
- DC1: Windows Server, 2GB.
- DC2 (second site): Windows Server, 2GB.
- SRV1 (file, DNS, DHCP, Windows Admin Center): Windows Server, 3GB.
- CLIENT1: Windows 11, 4GB.
- Host-only and NAT networks so you can test sites, DNS and DHCP.

**AZ-104 block:** mostly in Azure. Use a free account, set a budget alert first, and delete resource groups after each lab.

**Linux blocks:** 1-2 small VMs (1-2GB each): Debian/Ubuntu and a RHEL-family distro. Add a third for mail, DNS and web services in the LPIC-2 block.

## Weekly rhythm

- **Week 1 of each topic:** read the official skills outline, then video or course for the topic.
- **Middle weeks:** hands-on lab tied to each skills-measured bullet. Write down every step you did.
- **Last 2 weeks before an exam:** practice exams, review weak domains, book the exam.
- **Rule:** a topic isn't done until you can do it in the lab without notes.

## Sources

- [AZ-802 study guide](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/az-802)
- [AZ-104 study guide](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/az-104)
- [CompTIA Security+](https://www.comptia.org/en-us/certifications/security/)
- [CompTIA Linux+](https://www.comptia.org/en-us/certifications/linux/)
- [CompTIA Cloud+](https://www.comptia.org/en-us/certifications/cloud/)
- [LPIC-1](https://www.lpi.org/our-certifications/lpic-1-overview/), [LPIC-2](https://www.lpi.org/our-certifications/lpic-2-overview/), [LPIC-3](https://www.lpi.org/our-certifications/lpic-3-overview/)
