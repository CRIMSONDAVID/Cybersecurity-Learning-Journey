Learning Security Architecture
Introduction

In this journal entry I reflect on what I’ve learned about Security Architecture during my studies. The entry summarizes key concepts from my readings and guided reflections on how to design secure systems. I explain these ideas in simple terms and discuss how they fit into real-world cybersecurity work. The goal is to capture my understanding of topics like trust models, core security principles, governance, and design trade-offs.

What I Learned

Security Architecture: The overall blueprint or plan for protecting an organization’s IT systems and data. It’s how we arrange hardware, software, network designs, and policies to keep information safe. In other words, it’s the strategic design of systems, policies, and technologies that protect business assets
paloaltonetworks.com
A good security architecture aligns those protections with the company’s goals and risk levels.

CIA Triad: A foundational security model consisting of Confidentiality, Integrity, and Availability


Confidentiality means keeping data private – only authorized people can see or use it.
Integrity means keeping data accurate and unchanged unless properly modified (protecting it from unauthorized changes).
Availability means keeping systems and data up and running so authorized users can access them when needed.
Zero Trust: A security approach where no user or device is trusted by default – everyone must always prove they are allowed. This model “assumes breach” and checks every request as if it came from an untrusted network
learn.microsoft.com
In simple terms, Zero Trust teaches us to “never trust, always verify”
learn.microsoft.com
This means even someone inside the company network must re-authenticate or meet rules to use sensitive resources.

Governance: How leaders and policies guide cybersecurity across an organization. Governance is the framework of policies, oversight, and accountability that tells a company how to manage its security risks
threatlocker.com
In practice, it means executives and managers set security rules and ensure they match the organization’s objectives and legal requirements
threatlocker.com
Good governance connects day-to-day technical work to the company’s big-picture goals.

Security Trade-Offs: I learned that building secure systems often involves balancing competing goals. For example, making something very secure (with many checks) can make it harder or slower to use. Conversely, making a system super easy to use might leave gaps in security. One guide describes this as a trade-off between usability and security
cissecure.com
Recognizing these trade-offs helps designers decide the right level of controls and convenience.

Reflections
I found it interesting that Security Architecture isn’t just technical details but is tied to business needs. For example, I was surprised to learn that architects must align security controls with an organization’s goals
paloaltonetworks.com
Security isn’t only about firewalls and encryption; it also involves planning how a business should grow safely.

One thing that surprised me was how fundamental the CIA Triad is. I knew the terms, but seeing how Confidentiality, Integrity, and Availability cover almost every risk scenario was eye-opening
fortinet.com
It reminded me that security isn’t just locking data away: it’s also about keeping it correct and accessible.

The part I found hard to understand at first was governance. It seemed abstract to think about boards of directors in a technical topic. After studying it, I realized governance really means setting clear rules and responsibilities from the top
threatlocker.com
It bridges the “big picture” strategy with the work we do day-to-day to protect information.

These ideas apply to real cybersecurity work in many ways. For example, analysts often refer to the CIA triad when assessing risks or reporting to stakeholders. Engineers use trade-off thinking when deciding how strict logins or system locks should be, balancing security with user convenience. Governance comes into play whenever a company creates a security policy or reports compliance, showing that these concepts are part of everyday security jobs.
