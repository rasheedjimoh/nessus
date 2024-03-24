# Nessus Vulnerability Management

## Introduction

Welcome to my professional portfolio where I showcase my expertise in cybersecurity, specifically in vulnerability management using Nessus. Below, I'll guide you through the process of downloading, installing, and configuring Nessus on Ubuntu, and how it can be utilised for effective vulnerability management on Windows 10 hosts.

![before-remediation](https://github.com/rasheedjimoh/nessus/assets/157264080/908ab01a-068e-48ae-a031-97123896be3c)

## Why We Need It

In today's ever-evolving cybersecurity landscape, effective vulnerability management is essential to safeguarding organizational assets and maintaining a robust security posture. Here's why Nessus is indispensable:

1. **Comprehensive Vulnerability Assessment:**
   - Nessus offers a powerful vulnerability scanning capability, allowing organizations to conduct comprehensive assessments of their IT infrastructure. By identifying vulnerabilities across networks, systems, and applications, Nessus enables proactive risk mitigation and threat prevention.

2. **Prioritization of Security Risks:**
   - With Nessus, organizations can prioritize security risks based on severity and potential impact. By categorizing vulnerabilities and providing actionable insights, Nessus empowers security teams to focus resources on addressing the most critical threats, thereby enhancing overall security effectiveness.

3. **Detailed Reporting and Analysis:**
   - Nessus generates detailed reports that provide valuable insights into the security posture of the organization. These reports include comprehensive vulnerability assessments, remediation recommendations, and trend analysis, enabling informed decision-making and strategic planning for security enhancements.

4. **Automated Remediation Processes:**
   - Nessus supports automated remediation processes, allowing organizations to streamline vulnerability remediation efforts. By automating patching and configuration changes, Nessus helps reduce the window of exposure to security threats and minimizes the potential impact of vulnerabilities on the organization.

5. **Continuous Monitoring and Improvement:**
   - Nessus facilitates continuous monitoring of the organization's security posture, enabling ongoing vulnerability detection and remediation. By implementing regular scanning schedules and verification checks, Nessus supports a proactive approach to cybersecurity, ensuring that security measures remain effective over time.

In summary, Nessus plays a crucial role in enhancing organizational cybersecurity by providing comprehensive vulnerability management capabilities. By leveraging Nessus, organizations can proactively identify, prioritize, and remediate security vulnerabilities, thereby reducing the risk of security breaches and ensuring the resilience of their IT infrastructure.

## Nessus Installation and Configuration

1. **Download and Install Nessus:**
   - Begin by downloading Nessus from the official website and installing it on your Ubuntu system.
   ```bash
   wget https://www.tenable.com/downloads/nessus?loginAttempted=true
   sudo dpkg -i Nessus-10.7.1-ubuntu1404_amd64.deb
   ```

![Nessus-Downloading](https://github.com/rasheedjimoh/nessus/assets/157264080/4b4aa120-669c-4d4c-a3cb-4edb4e8bba40)


2. **Start Nessus Scanner:**
   - Start the Nessus Scanner service using the command below.
   ```bash
   /bin/systemctl start nessusd.service
   ```
![Nessus-Install](https://github.com/rasheedjimoh/nessus/assets/157264080/6c71bdda-d168-4756-bcd2-cb4ea66711cc)


3. **Configure Nessus Scanner:**
   - Access the Nessus Scanner interface via your browser to configure it.
   - Go to either https://itmanagementVM:8834/ or https://localhost:8834/ to access the configuration page.

![nessus-signin](https://github.com/rasheedjimoh/nessus/assets/157264080/badf4561-11dc-44ec-b300-d3aff63964a9)


Activating and Configuring Nessus:

1. **Turn Off Windows Firewall:**
   - Disable the Windows Firewall to allow Tenable through for effective scanning.

2. **Perform Non-Credential and Credentialed Scans:**
   - Initiate non-credential scans by inputting the host IP and scheduling the scan.
   - Set up and start credentialed scans for enhanced vulnerability detection and assessment.

![nessus-scan](https://github.com/rasheedjimoh/nessus/assets/157264080/db9559e5-863d-4147-91d4-ce11e29dc73f)

---

![before-remediation](https://github.com/rasheedjimoh/nessus/assets/157264080/908ab01a-068e-48ae-a031-97123896be3c)



## Enabling Credential Scan on Windows Hosts:

1. **Enable Remote Registry and Advanced Sharing:**
   - Enable Remote Registry and Advanced Sharing services on the Windows hosts.

2. **Adjust User Account Control (UAC) Settings:**
   - Change the User Account Control setting to "Never Notify" for seamless scanning.

3. **Modify Registry Settings:**
   - Navigate to the Registry Editor and modify the necessary settings to enable credential scanning.

By following these steps, you can effectively deploy and configure Nessus for vulnerability scanning and management, ensuring the security of your network infrastructure.

![after-remediation](https://github.com/rasheedjimoh/nessus/assets/157264080/f463ba5a-9168-49f5-9e25-2f2f6e93573e)


## Benefits and Integration

![nessus-scan-1](https://github.com/rasheedjimoh/nessus/assets/157264080/79cabb88-465e-4d07-8979-25d29f32659b)

Nessus is a powerful vulnerability scanner that integrates seamlessly into your cybersecurity framework, offering the following benefits:

- **Discover and Prioritize Vulnerabilities:** Identify and prioritise vulnerabilities based on their severity and potential impact.
- **Assess and Report:** Perform thorough vulnerability assessments and generate comprehensive reports for informed decision-making.
- **Remediate Vulnerabilities:** Develop automated remediation processes to address vulnerabilities efficiently, ensuring timely mitigation.
- **Verify Security Posture:** Validate the effectiveness of remediation efforts through verification scans, ensuring continuous improvement in security posture.

Nessus serves as a cornerstone in implementing vulnerability management functions, providing a robust solution for identifying, assessing, and remedying security vulnerabilities across your network infrastructure.


## Conclusion

By leveraging Nessus for vulnerability management, you can proactively identify and address security weaknesses, bolstering the resilience of your IT environment. Implementing automated remediation processes ensures timely response to emerging threats, enhancing overall cybersecurity posture.

Stay proactive, stay secure!
