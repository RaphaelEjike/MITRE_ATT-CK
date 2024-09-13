# Identifying and Mapping Threat Actors Using MITRE ATT&CK

Use the MITRE ATT&CK framework to compare and analyse a set of known threat actors. For example, threat actors in the finance industry. Map these adversaries’ tactics, techniques, and procedures (TTPs) against your organisation’s defences to determine if your security measures can effectively detect and respond to their attack patterns. This exercise will help ensure that your detection capabilities are aligned with the threats your organisation is most likely to face.

# Identifying and Mapping Threat Actors Using MITRE ATT&CK

### Introducing the ATT&CK Framework
MITRE's ATT&CK Framework is a powerful resource for enhancing defense strategies. This comprehensive database outlines real-world attack techniques, giving cybersecurity professionals a detailed playbook of adversarial methods. The framework breaks down the final stages of the kill chain into 12 categories, each covering various techniques used by attackers to infiltrate and move through networks.

### Categories in the ATT&CK Matrix
The 12 categories include: Initial Access, Execution, Persistence, Privilege Escalation, Defense Evasion, Credential Access, Discovery, Lateral Movement, Collection, Command and Control, Exfiltration, and Impact.

### Defending Against Behaviors, Not Tools
One of the key advantages of the ATT&CK Framework is its emphasis on adversarial behaviours rather than specific tools, which can change frequently. By focusing on the underlying tactics, techniques, and procedures (TTPs), organisations can create more resilient and adaptive security postures.

### Utilizing the ATT&CK Matrix
The ATT&CK Matrix can help identify security gaps and test network defences by simulating known attack techniques. For example, defenders can use the matrix to trace how high-profile attacks like WannaCry and NotPetya operated, enabling them to model these behaviours and strengthen their defences.

## Why Evaluate Your SOC?
Assessing your Security Operations Centre (SOC) is crucial to understanding where your strengths lie and where gaps exist in both your technology stack and operational processes. This evaluation will provide insights into how well your organisation can respond to threats if they were to materialise.

## The Pillars of a Strong SOC Foundation
- Operations: The day-to-day activities of the SOC.
- Procedures: Standard operating procedures (SOPs) that guide incident response.
- Tooling: The technology and information available to the SOC.
- Collaboration: The interaction within the SOC (across analysts, tiers, and leaders), with other departments (IT, Legal, PR), and external partners (MSPs, contractors).

## SOC Assessment Workflow
1 Threat Actor Research & ATT&CK TTP Mapping
- Map adversary TTPs using MITRE ATT&CK.

2 SIEM Detection Coverage Mapping
- Assess your SIEM’s detection rules and data sources using the ATT&CK Navigator to compare your current tech stack against mapped adversary techniques.

3 SIEM Detection Testing
- Test your detection rules using open-source tools like Caldera or Atomic Red Team, or commercial platforms like Mandiant’s SightGain. Delve into the search language used for detections and review the logs.

