
---

## Deliverables and evidence
- Network diagram showing topology and data flow
- Configuration files: Sysmon, NXLog/Winlogbeat, `inputs.conf` for UF
- Splunk saved searches and dashboard exports
- Screenshots: ingestion verification, alert firing, investigation queries, containment actions
- Example daily SOC summary report (PDF) and short demonstration video (2–3 minutes)

---

## Learning outcomes
By completing this lab you will be able to:
- Deploy and administer a Splunk instance and configure data inputs
- Configure endpoint telemetry (Sysmon) and forward logs reliably
- Write SPL queries for detection, aggregation, and correlation
- Simulate attacker behavior and map alerts to incident response steps
- Construct operational dashboards and produce regular SOC reporting
- Document incident triage and remediation in a reproducible playbook

---

## Status and next steps
**Current status:** repository scaffolded; VM and network setup pending.  
**Planned next steps:**
1. Create VirtualBox host-only network and provision VMs (Splunk, Windows, Linux, Kali)  
2. Install Splunk Enterprise on the Splunk VM and create indexes + TCP inputs  
3. Install Splunk UF on Linux endpoint and configure monitoring for `/var/log/auth.log`  
4. Install Sysmon on the Windows endpoint and configure NXLog/Winlogbeat to forward events to Splunk  
5. Implement and tune initial detections (brute-force, privilege escalation, PowerShell)  
6. Run attacker simulations, capture evidence, and finalize dashboards and reporting

---

## How to reproduce
1. Clone the repository.  
2. Create the host-only VirtualBox network `lab-net`.  
3. Provision four VMs and assign the IPs listed above.  
4. Follow the configuration files in `hosts/` and import the saved searches into Splunk.  
5. Run the simulation scripts in `simulations/` to verify detection and triage flows.

---

## Author
`n8develops` — Home SOC Lab: learning-by-building to demonstrate SOC operations skills for entry-level cybersecurity roles.

