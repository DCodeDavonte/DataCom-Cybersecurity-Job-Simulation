# 🛡️ Risk Assessment Report – Community Health Clinic

**Prepared by:** Davonte Johnson
**Role:** Cybersecurity Consultant  
**Client:** Community Health Clinic  
**Date:** 4/18/2025

---

## 1. Context

The client is a small community health clinic that provides primary care, lab testing, and basic mental health services to local residents. The clinic operates from a standalone facility that includes administrative offices, patient care areas, a records room, and a small server rack for internal systems.

To prevent unauthorized physical access, the clinic has installed a fence around the perimeter of its property and uses a padlock-secured gate at the main entrance. However, the leadership team is increasingly concerned about vulnerabilities related to their information systems, patient data, and digital infrastructure. They have requested a risk assessment to identify threats that could affect the confidentiality, integrity, or availability of their systems and records, as well as guidance on how to strengthen their current security posture.

---

## 2. Risk Matrix

| **Rating** | **Likelihood**            | **Consequence**             |
|------------|----------------------------|-------------------------------|
| 1          | Rare                      | Minimal impact              |
| 2          | Unlikely                  | Minor disruption            |
| 3          | Possible                  | Noticeable, recoverable impact |
| 4          | Likely                    | Major operational damage    |
| 5          | Almost certain            | Severe legal, financial, or reputational impact |

**Risk Score = Likelihood × Consequence**

| **Score Range** | **Risk Level** | **Definition**                                      |
|-----------------|----------------|-----------------------------------------------------|
| 1–4             | Low            | Minor concern, manageable risk                     |
| 5–9             | Moderate       | Acceptable with monitoring or minor controls       |
| 10–14           | High           | Needs mitigation and formal controls               |
| 15–19           | Very High      | Serious threat, must be addressed soon             |
| 20–25           | Extreme        | Critical risk; immediate action required           |


---

## 3. Identified Risk Scenarios

### 🔹 Scenario 1: Phishing Attack on Clinic Staff
A clinic employee receives a phishing email, clicks a malicious link, and unknowingly compromises system credentials. This could result in unauthorized access to PHI and internal systems.

- **Threat Actor:** External attacker  
- **Vulnerability:** Lack of awareness training, no MFA  
- **Asset at Risk:** Patient health records, internal email, clinic systems

### 🔹 Scenario 2: Physical Perimeter Breach
A section of the clinic’s perimeter fence is damaged or bypassed, allowing unauthorized individuals to enter the premises during off-hours.

- **Threat Actor:** Criminals or vandals  
- **Vulnerability:** Weak perimeter defense, no surveillance  
- **Asset at Risk:** PHI (paper or digital), devices, physical systems

### 🔹 Scenario 3: Insider Unauthorized Access
A staff member accesses patient records beyond their role-based permissions due to inherited access or insufficient enforcement of RBAC.

- **Threat Actor:** Internal employee  
- **Vulnerability:** Poor access control practices, lack of auditing  
- **Asset at Risk:** Electronic health records (EHR), PHI, compliance integrity

---

## 4. Inherent Risk Ratings (No Controls in Place)

| Scenario                   | Likelihood | Consequence | Risk Rating | Risk Level  |
|---------------------------|------------|-------------|-------------|-------------|
| Phishing Attack           | 5          | 4           | **20**          | **Extreme**     |
| Physical Perimeter Breach | 3          | 4           | **12**          | **High**        |
| Insider Unauthorized Access | 3        | 5           | **15**          | **Very High**   |

---

## 5. Current Risk Ratings (With Existing Controls)

| Scenario                   | Likelihood | Consequence | Risk Rating | Risk Level  |
|---------------------------|------------|-------------|-------------|-------------|
| Phishing Attack           | 3          | 4           | **12**          | **High**        |
| Physical Perimeter Breach | 2          | 4           | **8**           | **Moderate**    |
| Insider Unauthorized Access | 2        | 5           | **10**          | **High**        |

---

## 6. Target Risk Ratings (With Additional Controls)

| Scenario                   | Additional Measures                                 | Likelihood | Consequence | Risk Rating | Risk Level |
|---------------------------|-----------------------------------------------------|------------|-------------|-------------|------------|
| Phishing Attack           | MFA, awareness training, EDR                        | 2          | 4           | **8**           | **Moderate**   |
| Physical Perimeter Breach | Cameras, reinforced fencing, motion lighting        | 1          | 4           | **4**           | **Low**        |
| Insider Unauthorized Access | Access audits, least privilege, logging, offboarding | 1       | 4           | **4**           | **Low**        |

---

## 7. Summary of Recommendations

To further reduce risk, the following measures are recommended for implementation:

- **Security Awareness Training:** Conduct phishing simulations and regular training for all staff to improve recognition of malicious emails and attachments.
- **Multi-Factor Authentication (MFA):** Implement MFA on all user accounts to reduce the risk of credential compromise.
- **Endpoint Detection & Response (EDR):** Deploy endpoint protection capable of real-time threat detection, isolation, and rollback.
- **Perimeter Security Enhancements:** Install visible surveillance cameras, reinforce fencing, and add motion-activated lighting to deter unauthorized entry.
- **Access Control Improvements:** Apply the principle of least privilege, conduct regular access audits, and improve employee offboarding protocols.
- **Log Monitoring:** Enable system and access logging with periodic reviews for unusual access patterns or misuse.

---

## 8. Conclusion

This assessment highlights key vulnerabilities in the clinic’s current physical and digital security posture. While existing controls offer a moderate level of protection, several high-impact risks remain. By implementing the recommended security measures, the clinic can significantly lower the likelihood and impact of major security events, better comply with privacy regulations, and protect both patient trust and operational continuity.

