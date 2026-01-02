# Social-Engineering-Assignment
# Social Engineering & Phishing Analysis Write-Up

**Name:** Muhammad A’beed bin Firdaus  
**Student ID:** 52215124303  

---

## Overview
This repository documents phishing and social engineering analysis exercises completed on **TryHackMe**.  
The focus is on identifying phishing indicators, analyzing malicious email content, and safely handling suspicious URLs.

Objectives:
- Identify phishing vs legitimate emails  
- Understand common social engineering tactics  
- Analyze phishing email HTML content  
- Practice URL defanging for safe reporting  

---

## Exercise 1: The Phishing Pond

### Description
This exercise required reviewing multiple emails and determining whether each was **legitimate** or **phishing**, based on grammar, sender behavior, and embedded links.

### Analysis Results

| Email Case | Verdict | Reason |
|-----------|--------|-------|
| Email 1 | Legitimate | No grammar issues or suspicious links |
| Email 2 | Phishing | Domain impersonation (`r nicrosoft`) |
| Email 3 | Phishing | Unusual and unexpected request from a contact, possibly compromised|
| Email 4 | Phishing | Fake URL |
| Email 5 | Phishing | Requested enabling macros |
| Email 6 | Phishing | Credential-harvesting link |
| Email 7 | Phishing | Malicious fake link |
| Email 8 | Legitimate | No embedded links |
| Email 9 | Legitimate | Clean email, no suspicious URLs |
| Email 10 | Phishing | Requested national ID and bank details |

### Result
- All phishing emails were correctly identified  
- Flag obtained and exercise completed  

---

## Exercise 2: Phishing Emails in Action

### Description
This exercise involved analyzing real phishing email samples, identifying malicious URLs, and understanding attacker tracking techniques.

---

### Email Header Observation
- Sender email started with **`noreply`**, commonly used to appear automated and trustworthy in phishing campaigns

---

## HTML Email Analysis

### Extracted URLs
Examples found in the phishing email HTML:
- `http://devret.xyz/4833mt11254939vf6888zq22032si1269du1508rr`
- `http://devret.xyz/Creatives/Tracking.png`
- `http://devret.xyz/Creatives/unsub.png`
- `http://devret.xyz/4833fx11254939ea6888wk22032mk1269ep1508rr`
- `http://devret.xyz/4833jo11254939iz6888xo22032gu1269jm1508uu`

All URLs resolve to the same root domain.

---

## Root Domain Identification

**Root Domain:**
- devret.xyz
- defanged into devret[.]xyz

---

## Additional tasks
- Phishing email impersonated **Citrix**
- Netflix-themed phishing emails should be reported to the official Netflix phishing reporting page
- Technique used in the example to presuade the victim was urgency
- Email has to link url, instead it lead to an excel document that attempt to run regasms.exe

---

## Key Takeaways
- Phishing emails often use brand impersonation and urgency
- Legitimate organizations rarely request sensitive data via email
- URL defanging is essential for safe documentation
- Suspicious emails should always be reported to the impersonated organization

---

## Conclusion
This exercise improved practical skills in phishing detection, email analysis, and secure reporting.  
These skills are critical for defending against real-world social engineering attacks.

