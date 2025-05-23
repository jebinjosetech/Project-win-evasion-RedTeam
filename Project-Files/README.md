# Red Team Tactics

## Introduction
In today's evolving cybersecurity landscape, the threats are becoming more sophisticated and harder to detect. This project aims to examine and test the security of Windows systems, specifically focusing on understanding the capabilities and limitations of Windows Defender. By thoroughly testing Windows Defender, we can assess how well it protects against different cyber threats.

## Objectives
The primary objective of this project is to develop an innovative approach that integrates the MITRE ATT&CK Matrix with sophisticated red team techniques to identify and exploit security vulnerabilities within Windows 10 and Windows 11 operating systems.
## Pratical Implemenation 
We have split our practical sessions into three parts.

1)Metasolit Framework 
In this project, we use Metasploit to demonstrate how built-in security features of updated Windows systems detect and block non-FUD payloads. We generate a Windows reverse shell payload using msfvenom, host it on a local server, and attempt to download it via a web browser. The download request is intercepted by Windows Defender, which identifies the payload as malicious, leading to the file's quarantine and deletion. This demonstrates the effectiveness of modern security measures against non-FUD exploits.

2)Villian Framework 

In the second session, we demonstrate how the Villain framework is detected by the latest Windows security measures. Villain, effective before 2022, helped adversaries gain access to victim machines but is now easily detected by updated Windows Defender features. Despite its previous capabilities, Villain cannot bypass Windows 10/11 security due to robust features like real-time protection and User Account Control (UAC). The steps include cloning the Villain repository, generating a payload, and executing it in PowerShell. The Windows security system promptly detects and quarantines the payload, showcasing the advancements in Windows Defender's capabilities.

3)Real World Scenario (Our Situation)

In our final session, we demonstrate the real-world application of our Fully Undetectable (FUD) payload. Our scenario targets employees at XYZ company who lack cybersecurity knowledge. An adversary sends a phishing email with a malicious EXE file disguised as a security update. Once the employee executes the file on an updated Windows 10/11 machine, the FUD malware activates, granting the attacker access to the company laptop. The malware injects a PowerShell script as a background service and includes a feature to reconnect to the attacker's C2 server at random intervals. The attacker then bypasses User Access Control (UAC) prompts to gain full system control. Using Netcat, we demonstrate the payload's execution and its stealth operation, evading Windows Defender. The proof of concept confirms directory access on the compromised machine.





## Expected Outcomes
- Detailed report examining the efficacy of Windows Defender and identifying possible weaknesses within Windows 10 and 11.
- Creation of FUD payloads that can bypass the latest Windows security measures.
- An advanced red team strategy guide enhanced by the MITRE ATT&CK Matrix.
## Impact
This project will significantly impact cybersecurity by uncovering new insights into the security vulnerabilities of modern operating systems, aiding professionals in better predicting and defending against future cyber threats.

## Conclusion
The project aims to advance red team engagements and push the limits of current cybersecurity practices, providing deep insights and tools for better security measures.
## Environment Setup

### Prerequisites
- [**Windows 10/11 VM** with the latest updates](https://developer.microsoft.com/en-us/windows/downloads/virtual-machines/)
- **Kali Linux** attacker machine
    - [Kali Linux Cloud Access from Azure for WAN and real world scenario approch](https://azuremarketplace.microsoft.com/en/marketplace/apps/kali-linux.kali)
    - [Kali Linux VM for Local Lab and Demo/testing](https://www.kali.org/get-kali/#kali-virtual-machines)
- [**Python**: installed on both Windows and Kali Linux](https://www.python.org/downloads/)
- [**Docker**: Building and Hosting Mail server in Kali Linux](https://github.com/JOSHUAPBIJU/Project-winEvasion-Redteam/blob/main/Resource/Dockerfile) 
- [**PowerShell** with script execution policy set to unrestricted](https://learn.microsoft.com/en-us/answers/questions/506985/powershell-execution-setting-is-overridden-by-a-po)
- [**Administrator privileges** on the Windows system](https://support.microsoft.com/en-us/windows/how-do-i-log-on-as-an-administrator-63267a09-9926-991a-1c77-d203160c8563)
- [**Internet connection** for downloading necessary tools and scripts](#)
### Tools and Frameworks
- **MITRE ATT&CK Navigator**: [ATT&CK Navigator](https://mitre-attack.github.io/attack-navigator/)
- **Obfuscation tools**: For creating FUD payloads [will be updated soon..!]
- **C2 Framework**: In this project Azure Cloud server with kali Linux will act as a command and control for establishing connection with employee system[windows 11VM].
- **Villian Framework**:We are using the Villain framework to demonstrate how it fails against an updated Windows 11  machine with lastest security measures
- **Metaspolit Framework**:We are also using the Metasploit framework to demonstrate how an updated Windows 11 machine effectively defends against a malicious framework
- **PowerShell**: For scripting language
- **Vscode**: Programming IDE
- **Payload delivery**: Custom build Mail server runing in the same Azure Cloud server Kali Linux
- **PE2EXE**: For converting powershell [.ps1] payload to exe.
- ### Testing and Validation
- Conduct simulated attacks using the developed methodologies on test environments that closely resemble real-world scenarios.
- Use Kali Linux as the attacker machine and Windows 10 or 11 with updated defender security features as targets.
- Evaluate the effectiveness of the FUD payloads and document any detected vulnerabilities.

