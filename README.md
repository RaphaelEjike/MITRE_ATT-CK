# Identifying defence gaps and mapping threat actors using MITRE ATT&CK

Use the MITRE ATT&CK framework to compare and analyse a set of known threat actors. For example, the threat actors in the finance industry. Map these adversaries’ tactics, techniques, and procedures (TTPs) against your organisation’s defences to determine if your security measures can effectively detect and respond to their attack patterns. This exercise will help ensure that your detection capabilities are aligned with the threats your organisation is most likely to face.

### Introducing the ATT&CK Framework
MITRE's ATT&CK Framework is a powerful resource for enhancing defense strategies. This comprehensive database outlines real-world attack techniques, giving cybersecurity professionals a detailed playbook of adversarial methods. The framework breaks down the final stages of the kill chain into 12 categories, each covering various techniques used by attackers to infiltrate and move through networks.

### Defending Against Behaviors, Not Tools
One of the key advantages of the ATT&CK Framework is its emphasis on adversarial behaviours rather than specific tools, which can change frequently. By focusing on the underlying tactics, techniques, and procedures (TTPs), organisations can create more resilient and adaptive security postures.

### Utilizing the ATT&CK Matrix
The ATT&CK Matrix can help identify security gaps and test network defences by simulating known attack techniques. For example, defenders can use the matrix to trace how high-profile attacks like WannaCry and NotPetya operated, enabling them to model these behaviours and strengthen their defences.

# Step-by-Step Guide: Mapping Threat Actors Using MITRE ATT&CK

### 1. Identify Relevant Threat Actors
Research these groups to understand their TTPs (Tactics, Techniques, and Procedures). You can find detailed reports from sources such as Mandiant, Red Canary, and the Verizon DBIR or directily from MITRE ATT&CK. For the finance sector, these might include:
- APT Groups: admin@338, Indrik Spider, Lazarus Group, APT19, APT38
- Ransomware/eCrime Groups: Exotic Lily, FIN7, TA505

### 2. Access the MITRE ATT&CK Navigator
Go to the MITRE ATT&CK Navigator.

### 3. Select Threat Actor Profiles
In the Navigator, search for and load profiles of the threat actors you’ve identified. You can either:
- Manually map techniques based on your research.

| Cyber Kill Chain       | Mitre ATT&CK |
|--------------------------|---------------------|
|  Reconnaissance          |Reconnaissance |
| Weaponisation            | Execution|
| Delivery                 | Initial Access|
| Execution                | Initial Access|
| Installation             | Persistence / Defence Evasion|
| Command and control      | Command and control|
| Action on objectives     | Exfiltration  / Impact|
- OR use pre-built ATT&CK mappings of well-known groups (many reports on threat actors already reference ATT&CK techniques).



### 4. Overlay Your Defence Capabilities
Map your existing security controls and detection mechanisms against the techniques used by the selected threat actors. For example, if APT38 uses phishing (Initial Access) and credential dumping (Credential Access), check if your SIEM or security tools can detect and alert on these specific techniques.
#### To do this:
- List all your detection rules and the technologies (SIEM, EDR, IDS/IPS) you have in place.
- Identify the data sources (e.g., DNS logs, firewall logs, endpoint logs) that feed into these tools.

### 5. Identify Gaps
Compare the TTPs of the threat actors against your defences:
- If your security tools cover a technique (e.g., detecting credential dumping), mark it as "covered."
- If a technique is not covered, mark it as a gap. These are areas where your defences may be vulnerable to attack.

# Run these simulations in a controlled environment (or lab) to assess whether your security tools trigger alerts as expected

### 1. Test Your Detection Capabilities
After mapping the coverage, test the effectiveness of your defences:
- Open Source Tools: Use tools like Caldera or Atomic Red Team to simulate the attack techniques of the threat actors.
- Commercial Solutions: Tools like Mandiant SightGain can also test your detection rules.

### 2. Review Logs and Detection Rules
Go through your SIEM or detection logs to verify whether alerts were raised during the tests. If not, review the detection rules or write custom rules to improve your SOC’s ability to detect specific TTPs.

### 3. Continuously Monitor and Update
- Regularly monitor threat intelligence feeds and vendor reports to stay updated on emerging TTPs.
- Reassess your security posture every quarter or when significant changes occur in your organisation or the threat landscape.


# Reference 

- <a href="https://attack.mitre.org/">Mitre Att&ck</a>    
- <a href="https://youtube.com/playlist?list=PLLGRmm150VfBd_bk6fGqTqxr8SBeDcprb&si=HOCl3sKBg3I_xzLC">YouTube Mitre Att&ck Deep dive</a>
- <a href="https://mitre-attack.github.io/attack-navigator/">Mitre Att&ck Navigator</a> 





