# Nessus Vulnerability Management

Welcome to my professional portfolio where I showcase my expertise in cybersecurity, specifically in vulnerability management using Nessus. Below, I'll guide you through the process of downloading, installing, and configuring Nessus on Ubuntu, and how it can be utilised for effective vulnerability management on Windows 10 hosts.

Nessus Installation and Configuration:

1. **Download and Install Nessus:**
   - Begin by downloading Nessus from the official website and installing it on your Ubuntu system.
   ```bash
   wget https://www.tenable.com/downloads/nessus?loginAttempted=true
   sudo dpkg -i Nessus-10.7.1-ubuntu1404_amd64.deb
   ```

2. **Start Nessus Scanner:**
   - Start the Nessus Scanner service using the command below.
   ```bash
   /bin/systemctl start nessusd.service
   ```

3. **Configure Nessus Scanner:**
   - Access the Nessus Scanner interface via your browser to configure it.
   - Go to either https://itmanagementVM:8834/ or https://localhost:8834/ to access the configuration page.

Activating and Configuring Nessus:

1. **Turn Off Windows Firewall:**
   - Disable the Windows Firewall to allow Tenable through for effective scanning.

2. **Perform Non-Credential and Credentialed Scans:**
   - Initiate non-credential scans by inputting the host IP and scheduling the scan.
   - Set up and start credentialed scans for enhanced vulnerability detection and assessment.

Enabling Credential Scan on Windows Hosts:

1. **Enable Remote Registry and Advanced Sharing:**
   - Enable Remote Registry and Advanced Sharing services on the Windows hosts.

2. **Adjust User Account Control (UAC) Settings:**
   - Change the User Account Control setting to "Never Notify" for seamless scanning.

3. **Modify Registry Settings:**
   - Navigate to the Registry Editor and modify the necessary settings to enable credential scanning.

By following these steps, you can effectively deploy and configure Nessus for vulnerability scanning and management, ensuring the security of your network infrastructure.

Benefits and Integration:

Nessus is a powerful vulnerability scanner that integrates seamlessly into your cybersecurity framework, offering the following benefits:

- **Discover and Prioritize Vulnerabilities:** Identify and prioritise vulnerabilities based on their severity and potential impact.
- **Assess and Report:** Perform thorough vulnerability assessments and generate comprehensive reports for informed decision-making.
- **Remediate Vulnerabilities:** Develop automated remediation processes to address vulnerabilities efficiently, ensuring timely mitigation.
- **Verify Security Posture:** Validate the effectiveness of remediation efforts through verification scans, ensuring continuous improvement in security posture.

Nessus serves as a cornerstone in implementing vulnerability management functions, providing a robust solution for identifying, assessing, and remedying security vulnerabilities across your network infrastructure.

Conclusion:

By leveraging Nessus for vulnerability management, you can proactively identify and address security weaknesses, bolstering the resilience of your IT environment. Implementing automated remediation processes ensures timely response to emerging threats, enhancing overall cybersecurity posture.

Stay proactive, stay secure!
