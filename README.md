# elevate-labs-task3
Vulnerability Assessment using Nessus Essentials

In this project, I performed a full vulnerability assessment on my local system using Tenable Nessus Essentials, a widely used vulnerability scanning tool. The objective was to identify potential security weaknesses, analyze their severity, and document possible remediation steps.
I started by installing and setting up Nessus Essentials, activating it with the free educational license, and updating all the necessary plugins. Once the environment was ready, I created a Basic Network Scan, which serves as a full system vulnerability scan, and set the target as my local machine IP (localhost).
The scan was launched to analyze all active services, open ports, and potential configuration issues. The scanning process took approximately 30–60 minutes to complete. After completion, the tool generated a detailed vulnerability report highlighting 31 findings in total.
Out of these, 2 were Medium severity vulnerabilities, and 29 were Informational. The most critical issues detected were:
-SSL Certificate Cannot Be Trusted – caused by an untrusted or self-signed certificate.
-SMB Signing Not Required – which could allow man-in-the-middle (MITM) attacks on SMB traffic.
I analyzed each vulnerability, reviewed Nessus’s remediation suggestions, and researched potential fixes. These included replacing untrusted SSL certificates and enabling SMB signing in Windows Group Policy settings.
