This practice scenario involved analyzing a DDoS attack where the company’s internal network was flooded with ICMP packets. The traffic caused the network to stop responding for two hours. Investigation later revealed that an unconfigured firewall allowed the malicious ICMP traffic to enter the network. The incident management team applied emergency controls to contain the attack and restore essential operations.

What i was tasked to do:
  My task in this exercise was to review the incident using the NIST Cybersecurity Framework and document how the company handled each phase. I was required to analyze how the attack occurred, how it was contained, and what steps were taken to restore normal operations. I also evaluated the long-term improvements needed to strengthen network security.

Incident report analysis
Summary
This morning, the organisation experienced a slow response and the network services eventually stopped working due to normal network traffic analysis that could not access any network resources. This was due to a DDOS attack that compromised the internal network for two hours.
Identify
The cybersecurity team conducted an investigation on the security event and it was found that a malicious attacker had sent a malicious ICMP ping into the company’s network through an unconfigured firewall. This made the malicious attacker have access to the network through a distributed denial of service.
Protect
The security team had implemented a new firewall rule to reduce the rate of incoming ICMP packets, network monitoring software to detect abnormal traffic patterns, and IDS/IPS system to filter out some ICMP traffic based on suspicious characteristics.
Detect
To detect new unauthorized access attacks in the future, the team will use a
firewall logging tool and an intrusion detection system (IDS) to monitor all incoming traffic from the internet.
Respond
The security team contained the attack by blocking incoming ICMP packets, they took non- critical services offline, and restored critical services first. They discovered that the firewall was unconfigured and confirmed that ICMP flooding caused the outage.


Recover
After, the non-critical services was brought back online, and the whole network was ensured that it was working again. The team added a firewall rule to rate-limit ICMP, they also implemented networking tools and IDS\IPS to identify suspicious ICMP patterns. Policies were updated


