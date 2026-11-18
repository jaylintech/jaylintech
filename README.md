### JAYLIN HALTEMAN // `jaylin.tech`
**Systems Engineering · Endpoint & Identity Internals · Network Security & Diagnostics**

I build diagnostic tooling, network testbeds, and automation to isolate root causes across Windows internals, Active Directory, enterprise networking, and endpoint security.

[![Portfolio](https://img.shields.io/badge/Portfolio-jaylin.tech-0d9488?style=flat-square&logo=googlechrome&logoColor=white)](https://jaylin.tech)
[![Tech Notes](https://img.shields.io/badge/Field_Notes-notes.jaylin.tech-0f766e?style=flat-square&logo=readthedocs&logoColor=white)](https://notes.jaylin.tech)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Jaylin_Halteman-0284c7?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jaylin-halteman-7353531a8/)
[![Email](https://img.shields.io/badge/Contact-jaylin@jaylin.tech-334155?style=flat-square&logo=minutemailer&logoColor=white)](mailto:jaylin@jaylin.tech)

---

### Featured Projects & Tooling

| Repository | Focus Area | Key Stack & Capabilities |
| :--- | :--- | :--- |
| **[snowflake-inspired-webrtc-proxy-lab](https://github.com/jaylintech/snowflake-inspired-webrtc-proxy-lab)** | Network Security & Detection Engineering | Bounded WebRTC DataChannel proxy testbed in **Go**, multi-transport Docker harness (**Coturn TURN/TURNS**, **mitmproxy**, **Suricata**, **Zeek**), custom STUN/DTLS detection rules, and PCAP telemetry analyzers. |
| **[Windows-Scripts-Tools](https://github.com/jaylintech/Windows-Scripts-Tools)** | Windows Internals, AD & Endpoint Administration | Includes **[`Test-ADTrustAndIdentityState.ps1`](https://github.com/jaylintech/Windows-Scripts-Tools/tree/main/ActiveDirectory-GPO)** (LSA `$MACHINE.ACC` vs. AD `pwdLastSet` drift, `0x3e7` Kerberos cache auditing, ASN.1 CLDAP UDP probes), **[`Fix-QuickBooks.cmd`](https://github.com/jaylintech/Windows-Scripts-Tools/tree/main/Fix-QuickBooks)** Electron cache remediation, and M365/Outlook utilities. |

---

### Recent Technical Investigations ([notes.jaylin.tech](https://notes.jaylin.tech))

* **[Anatomy of a Broken Domain Trust: Auditing LSA `$MACHINE.ACC` Drift, `0x3e7` Kerberos Tickets, and Hidden Credential Overrides with PowerShell](https://notes.jaylin.tech/pages/auditing-ad-machine-trust-lsa-secrets-kerberos-powershell.html)** — Zero-mutation LSA secret inspection via `SeBackupPrivilege`, `SYSTEM` (`0x3e7`) Kerberos encryption auditing, and 38-byte ASN.1 BER CLDAP UDP probes.
* **[Phantom Terabytes: Investigating a 556 GB UniFi DPI Spike on the Dream Router 7](https://notes.jaylin.tech/pages/unifi-dream-router-7-dpi-1tb-ssl-spike-wireguard.html)** — Auditing embedded MongoDB (`ace_stat.stat_daily`) rollups vs. UI Traffic Identification anomalies.
* **[Repurposing a Samsung Note 20 Ultra as an AdGuard Home Server](https://notes.jaylin.tech/pages/repurposing-samsung-note-20-ultra-adguard-home-qemu-unifi.html)** — Unrooted Alpine Linux inside Termux/QEMU, isolated Services VLAN design, and UniFi DNAT recursion fixes.
* **[Snowflake-Inspired WebRTC Proxy PoC for Filter Evasion (Parts 1–3)](https://notes.jaylin.tech/pages/a-snowflake-inspired-webrtc-proxy-poc-for-filter-evasion-part-3.html)** — Empirical forward-proxy boundary testing, ALPN inspection behavior, and Suricata/EDR detection engineering.
* **[DNSFilter Agent: Wi-Fi Drops on Windows 11 24H2](https://notes.jaylin.tech/pages/dnsfilter-agent-wifi-issues-windows-11-24h2.html)** — Isolating `WLAN-AutoConfig` security restart loops (Event IDs `11004` / `11010`) on Intel AX201/AX211 adapters.
* **[New Outlook for Windows: Troubleshooting & Cache Reset Runbook](https://notes.jaylin.tech/pages/new-outlook-troubleshooting.html)** — Resolving `EBWebView` cache corruption and OAuth token loops.

---

### Core Technical Stack

- **Diagnostics & Security:** Windows/LSA/Kerberos Internals, Packet Analysis (Wireshark/PCAP), Suricata, Zeek, Sysmon, Event Forensics, SIP Signaling
- **Languages & Automation:** PowerShell (Win32 P/Invoke, ADSI, Raw Sockets), Go, Python, Batch, REST APIs
- **Infrastructure:** Active Directory / GPO, Microsoft 365, UniFi Routing & VLANs, Linux / Docker, Grandstream VoIP
