# Incident-handling-with-Splunk-weaponization-Phase

![image](https://github.com/user-attachments/assets/3809201f-4c33-4804-8973-58daf364e27b)

## Project Report: Investigating the Cyber Attack on Wayne Enterprises


### 1. Overview

Recently, Wayne Enterprises experienced a significant cyber attack. The attackers infiltrated their network, compromised their web server, and defaced their website, http://www.imreallynotbatman.com, displaying the message "YOUR SITE HAS BEEN DEFACED" along with their trademark. Wayne Enterprises engaged me as a Security Analyst to investigate the incident, identify the root cause, and trace all attacker activities within their network.

### 2. Weaponization Phase

During the weaponization phase, the adversaries typically create malicious documents or malware to gain initial access while evading detection. They also establish domains similar to the target domain to trick users and create a Command and Control Server for post-exploitation communication and activity.

During my investigation, I identified several domains and IP addresses associated with the attackers. Specifically, I discovered a domain, prankglassinebracket.jumpingcrab.com, linked to this attack. My first task was to determine the IP address tied to these domains, which may have been pre-staged to attack Wayne Enterprises.
3. OSINT Investigation

### Robtex Analysis:

Robtex, a Threat Intelligence site that provides information about IP addresses and domain names, was instrumental in my investigation. By searching for the domain prankglassinebracket.jumpingcrab.com on Robtex, I was able to identify some associated domains and subdomains. I then searched for the IP address 23.22.63.114 on the same site. This IP address was linked to several domains that appeared to mimic the Wayne Enterprises site, providing further insight into the attacker's strategy.

![image](https://github.com/user-attachments/assets/29b30f0b-fb40-4bad-a9f3-c196c4cda08f)

![image](https://github.com/user-attachments/assets/57598a0b-dd72-4fba-9710-6f0af5ec8f18)

Some domains/subdomains associated with this domain:

![image](https://github.com/user-attachments/assets/04231cad-98f4-4ec2-9f4e-1885ac12245d)

Next, I searched for the IP address 23.22.63.114 on this Threat Intel site.

![image](https://github.com/user-attachments/assets/45e095d8-83f7-4bbd-a246-985536ce4df3)

### VirusTotal Analysis:

I also used VirusTotal, an OSINT tool for analyzing suspicious files, domains, and IPs. By searching for the IP address on VirusTotal, I could explore the RELATIONS tab, where I found all the domains associated with this IP that resembled the Wayne Enterprises domain. Among these was a domain associated with the attacker, www.po1s0n1vy.com. A subsequent search for this domain on VirusTotal revealed valuable information, including Whois details, which I cross-referenced on whois.domaintools.com.

### 4. Findings and Analysis

Through diligent investigation, I found that the IP address 23.22.63.114 was linked to domains pre-staged to attack Wayne Enterprises. Moreover, by aggregating data from various open-source intelligence sources, I identified an email address, lillian.rose@po1s0nvy.com, most likely associated with the P01s0n1vy Advanced Persistent Threat (APT) group.

![image](https://github.com/user-attachments/assets/ce3ddb5c-141a-43bd-81df-76b298306a80)

![image](https://github.com/user-attachments/assets/3350f2bb-8d65-4c03-ba79-078fde8f2b98)

In the domain list, I saw the domain that is associated with the attacker www.po1s0n1vy.com

![image](https://github.com/user-attachments/assets/e65e93a3-6bb8-477e-b02b-0c46d5e6d947)

I also look for the whois information on this site -> whois.domaintools.com to see if we can find something valuable.

![image](https://github.com/user-attachments/assets/87e15844-d2df-4fe8-a8be-cec0d974dedf)


### 5. Conclusion

The cyber attack on Wayne Enterprises was a sophisticated and well-planned operation, involving the creation of deceptive domains, malicious IP addresses, and phishing tactics to infiltrate and deface the company's website. By leveraging OSINT tools like Robtex and VirusTotal, I was able to trace the attack back to the P01s0n1vy APT group and uncover critical details about their tactics, infrastructure, and potential future targets.

### 6. Experience Gained

This investigation provided me with valuable experience in tracking and analyzing advanced cyber threats. I deepened my understanding of the weaponization phase of cyber attacks and the use of OSINT tools to uncover hidden relationships between domains, IP addresses, and threat actors. Additionally, I honed my skills in using Threat Intelligence platforms like Robtex and VirusTotal to gather and correlate data crucial for identifying attackers and their methods.

### 7. Benefits

The insights gained from this investigation not only enhanced my technical expertise but also contributed to strengthening Wayne Enterprises' cybersecurity posture. By identifying and mitigating the root causes of the attack, I helped the organization implement stronger defenses, including enhanced monitoring, timely patching, and stricter password policies. This project also underscored the importance of proactive threat hunting and the use of OSINT in preventing and responding to cyber threats.

