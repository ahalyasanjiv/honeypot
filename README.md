# Project 9 - Honeypot

## Honeypots Deployed
I deployed 3 different types of honeypots (Dionaea, Snort, and Cowrie) using 3 virtual machines.

- **Dionaea over HTTP**: a low interaction, server side honeypot that tries to trap malware samples.

- **Snort**: an intrusion prevention system that can do real-time traffic analysis and packet logging.

- **Cowrie**: a honeypot that logs brute force attacks and the attacker's shell interaction.


## Issues encountered
One of the first issues I encountered was creating a project on my Google Cloud Platform account. I later realized that the particular Gmail account I was using was under an organization and did not allow for projects to be created, so I used another account instead.

The second issue I encountered happened when I was installing the MHN Admin Application. The Github repository that I cloned according to the instructions in the assignment had a faulty script (it was cloning a repository that no longer existed). The TA emailed us the fixed command for cloning the link from Github:

```
sudo git clone https://github.com/threatstream/mhn.git
```

The third issue I encountered was getting attacks to appear on the MHN application. After searching online for possible fixes, I followed instructions from a MHN Troubleshooting Guide (https://bit.ly/2rpXrM1) and decided to used the Zenmap application instead of ```nmap``` on the command line.

## Summary of Data Collected
- Number of Attacks: 3096
- Number of Malware Samples: 0


**Top 5 Attacker IPs**
1. 66.108.67.162 (144 attacks)
2. 109.248.9.103 (109 attacks)
3. 58.218.213.156 (97 attacks)
4. 142.93.6.77 (61 attacks)
5. 104.248.29.221 (58 attacks)

**Top 5 Attacks Signatures**
1. ET DROP Dshield Block Listed Source group 1 (158 times)
2. ET SCAN Sipvicious User-Agent Detected (friendly-scanner) (10 times)
3. ET SCAN Suspicious inbound to mySQL port 3306 (9 times)
4. ET SCAN Sipvicious Scan (9 times)
5. ET CINS Active Threat Intelligence Poor Reputation IP TCP group 10 (8 times)

## Unresolved Questions Raised by Data Collected
- What caused 26 attackers to have unknown IP addresses?
- Why was the "ET DROP Dshield Block Listed Source group 1" attack signature significantly more common than the rest?
