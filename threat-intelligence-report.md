# Overview

APT34 — also known as Helminth, Clayslide, IRN2, MUDDYWATER, and more commonly OilRig — is a well-documented Iranian threat actor active since at least 2014. These aliases originate from various cybersecurity vendors and industry communities but consistently point to the same actor. APT34 is widely understood to operate on behalf of the Iranian government, with a primary focus on cyber espionage rather than active disruption.

---

# History

Notable campaigns over the past decade include:

**May 2016**: A targeted spear phishing campaign against Middle Eastern banks involving customized scripts not typically seen in mainstream cybercrime. These operations focused on reconnaissance and information gathering.

**July–Late 2017**: Exploitation of Microsoft Office vulnerabilities to breach government organizations in the Middle East. Custom PowerShell backdoors such as POWRUNER and BONDUPDATER were deployed, enabling persistent access for further intelligence collection.

---

# Targeted Industries

APT34 has been known to consistently target specific Middle Eastern sectors and industries (MiTRE, Crowdstrike):

- Government  
- Financial Services  
- Energy  
- Telecommunications  
- Aerospace  
- Hospitality

---

# Motives

APT34 is primarily focused on cyber espionage. They seek to gather information surrounding a target and presumably provide that information to the Iranian government. In 2019, the technical director at the NSA’s Threat Operations Center emphasized that APT34’s operations are primarily concerned with espionage, not destruction (Cyberscoop, 2019). While disruption garners headlines, strategic access to sensitive government or industry data can be equally — if not more — impactful, especially when leveraged by a nation-state. This strong association can have dire consequences in the geopolitical sphere. APT34 has also been reported to target various U.S. assets in the past which presents a scope that extends beyond the Middle East. This also hints that gaining long-term access to sensitive or private information is likely a vital piece of their strategy. As previously mentioned, their actions closely align with those of Iran’s broader geopolitical goals and/or interests. However, by understanding and correlating APT34’s motives and actions, we can take a more defensive, yet proactive approach. This will not only provide short-term benefits, but potentially long-term, sturdier solutions.

---

# Tactics, Techniques, and Procedures (TTPs)

We can get a clearer understanding of APT34’s methods and strategies by applying our information on the group to the MITRE ATT&CK Matrix.

| **Phase**            | **Technique**                  | **MITRE ID** | **Notes**                                        |
|----------------------|--------------------------------|--------------|-------------------------------------------------|
| Initial Access        | Spear phishing Attachment      | T1566.001    | Commonly observed delivery method               |
| Execution             | PowerShell                     | T1059.001    | Often used in Helminth backdoor                 |
| Persistence           | Scheduled Task/Job             | T1053        | Ensures long-term access                        |
| Defense Evasion       | Obfuscated Files or Information| T1027        | Used to bypass detection                        |
| Credential Access     | Credential Dumping             | T1003        | Suspected in lateral movement                   |
| C2                   | Custom Command & Control        | T1071        | Encrypted communication with C2 infrastructure  |
| Supply Chain Abuse    | Trusted Relationship           | T1199        | Targets downstream partners to pivot to main victims |

---

# Recommendations for Risk Mitigation

There are various measures that the organization can take in order to mitigate the risks and tactics often associated with the APT34 threat group. The following outlines the most impactful strategies that we can implement:

---

## User Awareness & Access Control

- Conduct regular phishing and social engineering training for all employees.  
- Apply the Principle of Least Privilege to limit user access to only what is necessary.  
- Enable anomaly detection and account lockouts for suspicious login behavior.

---

## Email & Endpoint Protection

- Deploy advanced email filtering to detect and block phishing attempts and malicious attachments.  
- Restrict unauthorized downloads and script execution on endpoints.  
- Maintain up-to-date endpoint protection with real-time threat detection capabilities.

---

## Network Segmentation & Monitoring

- Segment the network using VLANs or subnetting to limit lateral movement.  
- Enforce firewall rules to control inbound/outbound traffic based on protocol and destination.  
- Monitor internal traffic for signs of unusual lateral activity or privilege escalation.

---

## Vendor & Supply Chain Security

- Conduct risk assessments for third-party vendors prior to access provisioning.  
- Restrict vendor access to only required systems or data.  
- Maintain a software inventory and enforce patching protocols for third-party tools.
