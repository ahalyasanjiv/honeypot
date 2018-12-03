# Project 9 - Honeypot

## Honeypot Deployed
I deployed 3 different types of honeypots (Dionaea, Snort, and Cowrie) using 3 virtual machines.
Dionaea over HTTP: ``` mhn-honeypot-1 ```
Snort: ``` mhn-honeypot-2 ```
Cowrie: ``` mhn-honeypot-1 ```


## Issues encountered
One of the first issues I encountered was creating a project on my Google Cloud Platform account. I later realized that the particular gmail account I was using tied to an organization and did not allow for projects to be created, so I used another account instead.

The second issue I encountered happened when I was installing the MHN Admin Application. The github that I cloned according to the instructions in the assignment had a faulty script (it was cloning a repository that no longer existed). The TA emailed us the fixed command for cloning the link from Github:

```
sudo git clone https://github.com/threatstream/mhn.git
```

The third issue I encountered was getting attacks to appear on the MHN application. Instead of using ```nmap``` on the command line, I used the Zenmap application instead.

## Summary of Data Collected
Number of Attacks: 562
Number of Malware Samples: 0


TOP 5 Attacker IPs:
1. 66.108.67.162 (144 attacks)
2. [?] (26 attacks)
3. 167.99.133.253 (11 attacks)
4. 104.248.29.221 (9 attacks)  
5. 104.248.61.100 (8 attacks)

TOP 5 Attacks Signatures:
1. ET DROP Dshield Block Listed Source group 1 (12 times)
2. ET SCAN Suspicious inbound to PostgreSQL port 5432 (3 times)
3. ET SCAN NMAP OS Detection Probe (2 times)
4. ET CINS Active Threat Intelligence Poor Reputation IP UDP group 92 (1 times)
5. ET SCAN Suspicious inbound to MSSQL port 1433 (1 times)

## Unresolved Questions Raised by Data Collected
