How I Conducted a Security Audit for Botium Toys (NIST CSF Framework)
Project Overview

Botium Toys is a (fictional) growing toy company that recently expanded its online sales and is moving into the European market. This rapid growth and EU expansion triggered the need for a thorough IT security audit, especially to meet GDPR requirements for EU customers. The audit scope covered all of Botium’s IT resources – on-site servers, employee devices, e-commerce systems, network infrastructure, data storage, etc. – because the company’s official Scope and Goals report defines the audit as the “entire security program”. Using the NIST Cybersecurity Framework (CSF) as guidance, I assessed Botium’s security posture to identify strengths and gaps in its controls.

Framework and Materials Used
NIST Cybersecurity Framework (CSF) – This industry standard framework provides best practices for managing cybersecurity risk. As the FTC notes, NIST CSF “helps businesses of all sizes better understand, manage, and reduce their cybersecurity risk”. I used NIST CSF’s five core functions (Identify/Protect/Detect/Respond/Recover) to structure the audit.
Botium Toys: Scope, Goals, and Risk Assessment Report – An internal project document that defines the audit scope (all assets) and summarizes initial findings. It explicitly states that the audit covers “the entire security program at Botium Toys” with goals to “assess existing assets and complete the controls and compliance checklist to determine which controls… need to be implemented”.

Control Categories – A reference listing the NIST CSF control categories and descriptions (from course materials). This helped me understand each control’s purpose when filling out the checklist.
Controls & Compliance Checklist – The official audit template listing specific security controls and compliance best practices. I used this to mark which controls Botium currently has. 

Step-by-Step Audit Process
Review Scope & Assets: I began by studying the Scope and Risk report to understand exactly what Botium’s IT group manages. The report lists all assets under IT – on-premises servers and network equipment, employee laptops and mobile devices, point-of-sale and e-commerce systems, vendor-managed services, internal networks, and even legacy systems. Cataloguing these assets ensured that no important system (e.g. the credit-card database or customer PII storage) was overlooked.

Review Risk Assessment: 
Next I examined the risk assessment section. It highlighted major vulnerabilities: for example, “Botium Toys does not have all of the proper controls in place and may not be fully compliant with U.S. and international regulations”. The assessment even gave Botium a risk score of 8/10 due to these gaps. Notably, it pointed out that all employees could access internal data (including credit card and personal data) and that no encryption was used on payment data. These findings made it clear that data privacy and access controls were high priorities.
Map to NIST CSF Categories: With assets and risks identified, I mapped each finding to NIST CSF’s core functions (Identify, Protect, Detect, Respond, Recover). For example, creating the asset inventory fell under Identify, enabling firewalls and encryption fell under Protect, and checking for an intrusion-detection system fell under Detect. This mapping ensured a comprehensive view: every security aspect fit into one of the recognized CSF categories.

Key Takeaways
Structured Framework is Valuable: Using the NIST CSF gave a clear structure to the audit. Its five core functions (Identify/Protect/Detect/Respond/Recover) ensured we covered all areas of security, just as official guidance suggests.
Documentation Drives Focus: 
The initial scope and risk report was invaluable. It highlighted exactly where Botium’s weaknesses lay (e.g. missing encryption or backups, which focused the audit on those gaps rather than guessing.
Checklist Translates Theory to Action: 
Working through a controls checklist made the process concrete. Abstract ideas like “protect data” became specific questions (“Is data encrypted? Are backups done?”), which is very helpful for beginners.
Compliance Matters: 
I learned how business context affects security needs. Because Botium is entering the EU, GDPR requirements had to be checked. This shows that security isn’t just technical – you must also consider legal standards.

Reflective Practice: 
Overall, this exercise helped me connect coursework to reality. I saw how a mock audit can identify real risks, prioritize fixes, and justify them to stakeholders. It built my confidence in using NIST CSF to assess and improve a company’s security posture.

Reflection
This audit project was a great learning experience. Working through each step – from inventorying assets to mapping them to NIST CSF categories – made the framework’s concepts much clearer in a practical way. It reinforced how important it is to document and think critically: simply following the checklist turned a broad task into concrete questions with clear answers. I also saw firsthand that missing controls (like no disaster recovery plan) directly translate into business risk and compliance issues. In short, this project turned theory into practice and deepened my understanding of cybersecurity assessments.

Security incident report 
 
Section 1: Identify the network protocol involved in the incident 
The network protocol involved in the incident was both DNS and HTTP.  
For DNS, the browser had to look for the domains by requesting the IP 
addresses during the incident. This included the original domain 
(yummyrecipesforme.com) and the malicious redirect domain 
(greatrecipesforme.com) 
HTTP protocol retrieved the webpage and the downloaded the executable file. 
The HTTP requests also included the redirection traffic that occurred after the 
malware executed. 
 
Section 2: Document the incident 
 How the intrusion happened 
It happened that a former employee gained unauthorized access to the 
website’s hosting environment by performing a brute-force attack against the 
administrative login. Because the account was still using a default password 
and there were no protections in place to limit repeated login attempts, the 
attacker was able to successfully guess the credentials and enter the admin 
dashboard. 
 
What did the attacker change? 
After gaining access, the attacker modified the website’s source code by 
embedding a malicious JavaScript function. This script forced website visitors 
to download and run an executable file disguised as a browser update. Once 
executed, the file redirected users to a fake website (greatrecipesforme.com) 
that hosted additional malware. 
 
What thee customers had experienced 
After some hours, the customers reported that the website asked  them to 
download a file to access free recipes. After running the file, users noticed that 
their browsers redirected to a different URL and their computers operated 
more slowly. 
A sandbox was used to check the behavior while capturing traffic with 
tcpdump. The logs showed normal DNS and HTTP requests to the original 
domain followed by additional DNS and HTTP traffic to the fake domain. A 
senior analyst confirmed the code injection by reviewing the website’s source 
files and identified embedded JavaScript. This information served as evidence 
of the compromise. 
 
Section 3: Recommend one remediation for brute force attacks 
Implementing a policy that requires frequent password changes for the 
administrative account 
