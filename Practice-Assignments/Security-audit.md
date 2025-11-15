How I Conducted a Security Audit for Botium Toys (NIST CSF Framework)
Project Overview
Botium Toys is a (fictional) growing toy company that recently expanded its online sales and is moving into the European market. This rapid growth and EU expansion triggered the need for a thorough IT security audit, especially to meet GDPR requirements for EU customers. The audit scope covered all of Botium’s IT resources – on-site servers, employee devices, e-commerce systems, network infrastructure, data storage, etc. – because the company’s official Scope and Goals report defines the audit as the “entire security program”. Using the NIST Cybersecurity Framework (CSF) as guidance, I assessed Botium’s security posture to identify strengths and gaps in its controls.
Framework and Materials Used
NIST Cybersecurity Framework (CSF) – This industry standard framework provides best practices for managing cybersecurity risk. As the FTC notes, NIST CSF “helps businesses of all sizes better understand, manage, and reduce their cybersecurity risk”. I used NIST CSF’s five core functions (Identify/Protect/Detect/Respond/Recover) to structure the audit.
Botium Toys: Scope, Goals, and Risk Assessment Report – An internal project document that defines the audit scope (all assets) and summarizes initial findings. It explicitly states that the audit covers “the entire security program at Botium Toys” with goals to “assess existing assets and complete the controls and compliance checklist to determine which controls… need to be implemented”.
Control Categories – A reference listing the NIST CSF control categories and descriptions (from course materials). This helped me understand each control’s purpose when filling out the checklist.
Controls & Compliance Checklist – The official audit template listing specific security controls and compliance best practices. I used this to mark which controls Botium currently has. The checklist prompts questions like “Does Botium Toys currently have this control in place?”
studocu.com
 for each item, ensuring a systematic evaluation.
Step-by-Step Audit Process
Review Scope & Assets: I began by studying the Scope and Risk report to understand exactly what Botium’s IT group manages. The report lists all assets under IT – on-premises servers and network equipment, employee laptops and mobile devices, point-of-sale and e-commerce systems, vendor-managed services, internal networks, and even legacy systems. Cataloguing these assets ensured that no important system (e.g. the credit-card database or customer PII storage) was overlooked.
Review Risk Assessment: Next I examined the risk assessment section. It highlighted major vulnerabilities: for example, “Botium Toys does not have all of the proper controls in place and may not be fully compliant with U.S. and international regulations”. The assessment even gave Botium a risk score of 8/10 due to these gaps. Notably, it pointed out that all employees could access internal data (including credit card and personal data) and that no encryption was used on payment data. These findings made it clear that data privacy and access controls were high priorities.
Map to NIST CSF Categories: With assets and risks identified, I mapped each finding to NIST CSF’s core functions (Identify, Protect, Detect, Respond, Recover). For example, creating the asset inventory fell under Identify, enabling firewalls and encryption fell under Protect, and checking for an intrusion-detection system fell under Detect. This mapping ensured a comprehensive view: every security aspect fit into one of the recognized CSF categories.
Complete Controls & Compliance Checklist: I then systematically went through the Controls checklist, answering Yes/No for each control. For instance, Botium already had a network firewall and antivirus in place (so those were marked Yes), whereas it lacked formal plans and systems in other areas. The report explicitly notes “There are no disaster recovery plans currently in place, and the company does not have backups of critical data.”
cdn3.f-cdn.com
, so those items were marked No. Because Botium is expanding into Europe, I also checked compliance items: the EU’s GDPR rules became relevant and currently were not fully implemented, so GDPR compliance was flagged No. This step-by-step checklist made it easy to see which controls were in place and which were missing.
Recommendations for Improvement: Finally, I formulated recommendations to address each gap. For example, since least-privilege access was not enforced (employees had broad data access), I recommended implementing strict access controls. I also advised encrypting sensitive data at rest (the report noted “Encryption is not currently used” for credit cards), and establishing a formal incident response/disaster recovery plan (none existed
cdn3.f-cdn.com
). Other suggestions included enforcing strong password policies and strengthening GDPR/privacy controls. Each recommendation corresponded to a CSF function and directly addressed a risk identified earlier.
Sample Results
As an example, the completed checklist might summarize key categories like this:
Control Category	In Place?
Access Control	Yes
Data Security	Yes
Network Monitoring (IDS)	No
Incident Response Plan	No
Regulatory Compliance (GDPR)	No
In this sample, controls for access management and basic data security were present, but network monitoring and incident response capabilities were missing. GDPR compliance was also marked No, reflecting the need to improve privacy practices for EU data.
Key Takeaways
Structured Framework is Valuable: Using the NIST CSF gave a clear structure to the audit. Its five core functions (Identify/Protect/Detect/Respond/Recover) ensured we covered all areas of security, just as official guidance suggests.
Documentation Drives Focus: The initial scope and risk report was invaluable. It highlighted exactly where Botium’s weaknesses lay (e.g. missing encryption or backups
cdn3.f-cdn.com
), which focused the audit on those gaps rather than guessing.
Checklist Translates Theory to Action: Working through a controls checklist made the process concrete. Abstract ideas like “protect data” became specific questions (“Is data encrypted? Are backups done?”), which is very helpful for beginners.
Compliance Matters: I learned how business context affects security needs. Because Botium is entering the EU, GDPR requirements had to be checked. This shows that security isn’t just technical – you must also consider legal standards.
Reflective Practice: Overall, this exercise helped me connect coursework to reality. I saw how a mock audit can identify real risks, prioritize fixes, and justify them to stakeholders. It built my confidence in using NIST CSF to assess and improve a company’s security posture.
Files Attached
The following documents are included in this folder for reference and completeness:
ScopeGoals_RiskReport.pdf – The Botium Toys Scope, Goals, and Risk Assessment report (original audit document).
Controls_Compliance_Checklist.pdf – The completed controls and compliance checklist with Yes/No answers
Any additional supporting files (e.g. Control Categories reference) are also included for context.
Each file contains the detailed work products mentioned above, so reviewers can see exactly how the checklist was filled out and what evidence supported our conclusions.
Reflection
This audit project was a great learning experience. Working through each step – from inventorying assets to mapping them to NIST CSF categories – made the framework’s concepts much clearer in a practical way. It reinforced how important it is to document and think critically: simply following the checklist turned a broad task into concrete questions with clear answers. I also saw firsthand that missing controls (like no disaster recovery plan) directly translate into business risk and compliance issues. In short, this project turned theory into practice and deepened my understanding of cybersecurity assessments.
