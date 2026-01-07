# Rules of Engagement (RoE)

**Client:** [Company Name]
**Consultant/Pentester:** [Your Name]
**Date:** [MM/DD/YYYY]

---

## 1. Testing Window
Definition of allowed timeframes for test execution.

- [ ] **24/7:** Testing allowed at any time.
- [ ] **Business Hours:** Only from 09:00 to 18:00 (Mon-Fri).
- [ ] **After Hours:** Only after 19:00 or weekends.
- [ ] **Other:** ________________________

## 2. Exploitation Techniques
What is allowed and what is strictly prohibited during the engagement.

| Technique | Allowed? | Notes |
| :--- | :---: | :--- |
| **Active Exploitation** | YES / NO | Running exploits that may crash services. |
| **Social Engineering** | YES / NO | Phishing, Vishing, SMS attacks. |
| **Physical Access** | YES / NO | Attempting to enter offices/server rooms. |
| **DoS / Stress Test** | YES / NO | Denial of Service attacks. |
| **WAF/IPS Bypass** | YES / NO | Evasion techniques against firewalls. |
| **Data Exfiltration** | YES / NO | Extracting real PII data for Proof of Concept. |

## 3. Communication & Emergency
In case a critical service goes down or an intrusion is detected by the Blue Team.

* **Primary Contact (Client):**
    * Name: __________________
    * Phone (24h): __________________
    * Email: __________________

* **Primary Contact (Consultant):**
    * Name: [Your Name]
    * Phone: [Your Phone]

## 4. Evidence Handling
* Should screenshots of sensitive data be anonymized in the final report? (Yes/No)
* Must extracted data (DB dumps) be deleted immediately after verification? (Yes/No)

## 5. Post-Engagement Cleanup
The consultant commits to removing:
* Installed shells/backdoors.
* Test user accounts.
* Temporary files or scripts.

---
**Signatures:**

__________________________
[Client Representative]

__________________________
[Consultant Name]
