# Project-win-evasion-RedTeam
The project, titled "RED TEAM TACTICS," was built by [Jebin Jose](https://github.com/jebinjosetech) . I have successfully completed this project with a top-level grade (Grade 1)
> [!NOTE]
> This project integrates the MITRE ATT&CK framework with advanced red team tactics to identify and exploit security vulnerabilities in Windows systems.

> [!TIP]
> Use PowerShell scripts with advanced obfuscation techniques to create Fully Undetectable (FUD) payloads that can bypass Windows Defender.

> [!IMPORTANT]
> Regular updates to FUD payloads are necessary to keep up with the latest Windows security features and ensure continued effectiveness.
## Attack - EVENT TIME LINE

![Att&ck Time Line](https://raw.githubusercontent.com/jebinjosetech/Project-win-evasion-RedTeam/main/Resource/attack-time-line.png)

### Scenario :
_An adversary attempts to send a phishing email to technical support Employees of a XYZ company . One of the employees, who lacks cybersecurity knowledge, opens the email and downloads an attached file. The file is a password-protected ZIP archive. The employee manages to unzip the file and install or test the content within it.
Meanwhile, the adversary gains access to the employee's company laptop. The adversary delivers a PowerShell script disguised as an executable (EXE) file. This script downloads a PowerShell script (PS1) from a cloud server into memory and executes it, bypassing detection by the employee and the default Windows security mechanisms.
The PowerShell script is obfuscated to evade antivirus detection. Once the obfuscated script is running in memory, it gains access to the laptop and spams UAC (User Account Control) prompts to obtain administrative rights. After successfully bypassing UAC, the adversary gains full control over the system._
> [!IMPORTANT]
> Find [MITRE ATT&CK for Scenario](https://github.com/jebinjosetech/Project-win-evasion-RedTeam/blob/main/MITRE%20ATT%26CK/README.md)

> [!IMPORTANT]
> ATT&CK Navigator File

[Attack json file | download ](https://github.com/jebinjosetech/Project-win-evasion-RedTeam/blob/main/MITRE%20ATT%26CK/adversary_tactics_and_techniques_for_hacking_win11-10_using_phishing_scenario.json) upload to [ATT&CK Navigator](https://mitre-attack.github.io/attack-navigator/) for customization or for better view.
+ MITRE ATT&CK®
![MITRE ATT&CK®](https://github.com/jebinjosetech/Project-win-evasion-RedTeam/blob/main/Resource/Adversary_Tactics_and_Techniques_for_Phishing_Scenario(3).svg)
- [x] The above attack can be improvised 
- [ ] Effort calculated:- 300+ hours 🕙 in 5 months 📆 	`Approximate value`
- [ ] Add delight to the experience when all tasks are completed
> [!WARNING]
> Simulated attacks in this project reveal potential vulnerabilities that adversaries might exploit, emphasizing the need for robust cybersecurity measures.

> [!CAUTION]
> This project demonstrates sophisticated cyber-attacks, and its findings should be used responsibly to enhance defensive strategies and improve system security.
> ### Attack and C2 Setup 
  1. [Ubuntu Server Configuration for C2 and Mail Server](https://github.com/jebinjosetech/Project-win-evasion-RedTeam/blob/main/Resource/ubuntu-server-config-for-C2-mailserver.md)
  2. [Powershell Script to Payload.exe](https://github.com/jebinjosetech/Project-win-evasion-RedTeam/blob/main/Resource/powershell-script-2-exe.md)
  3. [Python Script for Sending Mail with Payload.exe](https://github.com/jebinjosetech/Project-win-evasion-RedTeam/blob/main/Resource/mail-sending-python-script.md)
  4. [Metasploit Payload Generating](https://github.com/jebinjosetech/Project-win-evasion-RedTeam/blob/main/Resource/mataspolit-payload-gen-step.md)
  5. [Villain Payload](https://github.com/jebinjosetech/Project-win-evasion-RedTeam/blob/main/Resource/villian-payload-genstep.md)
  6. [Windows dwfender analysis scrpit](https://github.com/jebinjosetech/Project-win-evasion-RedTeam/blob/main/Resource/Windows-Defender-script.md)
### **References**

  1. [scenario reference-01](https://www.techopedia.com/antivirus/antivirus-statistics)
  2. [scenario reference-02](https://www.malwarebytes.com/blog/news/2020/10/work-devices-for-personal-use)
  3. [MITRE ATT&CK®](https://attack.mitre.org/)
  4. [Attack-Naigator](https://mitre-attack.github.io/attack-navigator/)
  5. [Windows 10/11 security update](https://techcommunity.microsoft.com/t5/windows-servicing/updates-so-often/m-p/39526)
  6. [Villian Framework](https://github.com/t3l3machus/Villain)
  7. [Metaspolit Framework](https://www.metasploit.com/)
  
You can access the [Report](https://github.com/jebinjosetech/Project-win-evasion-RedTeam/blob/main/Resource/IT_SEC_REPORT.pdf) for more details.
 
