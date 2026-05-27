# Lab: Compare Penetration Testing Methodologies

## Course
Cisco Ethical Hacker – Module 1.2.6

## Objective
The goal of this lab was to compare different penetration testing and security assessment frameworks and understand how each one is used in practice.

---

## Methodologies Compared

### 1. PTES (Penetration Testing Execution Standard)

#### Overview
PTES is a structured framework that guides penetration testers through the full testing process, starting from planning and ending with reporting.

#### Main Phases
- Pre-engagement interactions
- Intelligence gathering
- Threat modeling
- Vulnerability analysis
- Exploitation
- Post-exploitation
- Reporting

#### Key Points
- Covers the complete penetration testing lifecycle
- Helps keep assessments organized
- Focuses on realistic attack simulation
- Gives importance to documentation and reporting

#### My Understanding
PTES feels like a proper roadmap for penetration testing. Instead of testing randomly, it gives a clear sequence to follow, which makes the work more professional and easier to manage.

---

### 2. OWASP Web Security Testing Guide (WSTG)

#### Overview
OWASP WSTG is a guide for testing the security of web applications and web services.

#### Areas Covered
- Input validation
- Authentication
- Session management
- Authorization
- Security misconfigurations
- Client-side security

#### Key Points
- Designed specifically for web security testing
- Very useful in bug bounty and web application assessments
- Practical and checklist-based
- Updated by the security community

#### My Understanding
OWASP WSTG is one of the most useful guides for website security testing. It is practical, easy to follow, and especially helpful when checking common web vulnerabilities.

---

### 3. OSSTMM (Open Source Security Testing Methodology Manual)

#### Overview
OSSTMM is a security testing methodology that focuses on measuring operational security across different environments.

#### Areas Covered
- Network security
- Wireless security
- Physical security
- Telecommunications
- Human security

#### Key Points
- Covers more than just technical testing
- Includes measurement and analysis
- Useful for broader security assessments
- Focuses on operational security

#### My Understanding
OSSTMM is broader than a normal pentesting guide. It looks at security from a wider point of view and reminds us that security is not only about systems, but also about people and processes.

---

### 4. MITRE ATT&CK

#### Overview
MITRE ATT&CK is a knowledge base of real-world attacker tactics and techniques. It is widely used to understand how attackers behave after gaining access to a system.

#### Areas Covered
- Initial access
- Execution
- Persistence
- Privilege escalation
- Credential access
- Defense evasion
- Lateral movement
- Data exfiltration

#### Key Points
- Based on real attacker behavior
- Widely used in threat detection and incident response
- Helpful for blue teams and SOC analysts
- Shows how attacks progress step by step

#### My Understanding
MITRE ATT&CK stood out to me because it focuses on attacker behavior in a practical way. It helps security teams understand what an attacker may do after entering a system, which makes detection and defense much easier.

---

## Comparison Summary

| Feature | PTES | OWASP WSTG | OSSTMM | MITRE ATT&CK |
|---|---|---|---|---|
| Main Focus | Full pentesting lifecycle | Web application security | Operational security testing | Attacker tactics and techniques |
| Scope | General penetration testing | Web applications | Multiple environments | Real-world attack behavior |
| Style | Structured process | Checklist-based | Measurement-oriented | Technique and behavior mapping |
| Common Use | Professional pentests | Web security assessments | Security audits | Detection, defense, and incident response |

---

## Key Observations
- PTES provides a clear and complete process for penetration testing.
- OWASP WSTG is the most useful for web application security testing.
- OSSTMM covers a wider security scope, including physical and human factors.
- MITRE ATT&CK is useful for understanding how attackers operate in real environments.
- Each framework serves a different purpose, so the choice depends on the type of assessment.

---

## What I Learned
This lab helped me understand that cybersecurity testing is not done randomly. Different frameworks exist for different goals, and each one helps security professionals work in a more organized way.

I also learned that:
- Web testing needs specialized guidance
- Security assessments can include more than just technical systems
- Real attacker behavior is important for detection and defense
- Documentation and planning are important in pentesting

---

## Conclusion
This lab improved my understanding of major penetration testing and security assessment frameworks. PTES gives a full testing workflow, OWASP WSTG focuses on web applications, OSSTMM covers broader operational security, and MITRE ATT&CK helps explain real attacker behavior. Together, these frameworks show that effective cybersecurity work depends on structure, observation, and planning.
