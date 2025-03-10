# Elastic-Defense-Lab

## 📌 Project Overview
Elastic-Defense-Lab is a **cybersecurity home lab** designed to simulate real-world **SOC (Security Operations Center) analyst** tasks. It leverages **AWS, Windows, Elastic SIEM, and Elastic Defend** to detect and respond to malware, providing hands-on experience in threat monitoring and incident response.

## 🛠 Tools & Technologies Used
- **AWS EC2** – Windows instance for endpoint monitoring
- **Elastic SIEM** – Cloud-based security information and event management
- **Elastic Defend** – Endpoint Detection & Response (EDR) solution
- **Windows Event Logs** – Log collection for security analysis
- **PowerShell** – Agent installation and configuration

## 🚀 Features
- Deploys a **Windows virtual machine** in AWS
- Installs **Elastic Defend** for endpoint monitoring
- Configures **Elastic SIEM** to collect and analyze logs
- Simulates **malware detection** using the EICAR test file
- Responds to threats **just like a SOC analyst**

## 🏗️ Setup Instructions
### **1️⃣ Deploy Windows Instance in AWS**
1. Create an **AWS account** ([AWS Free Tier](https://aws.amazon.com/free/)).
2. Launch a **Windows EC2 instance** using a free-tier eligible AMI.
3. Create and download an **RDP key pair** to access your instance.
4. Configure security groups to allow **RDP access (port 3389)**.
5. Connect to the instance using **Remote Desktop Protocol (RDP)**.

📸 **User Screenshot (Elastic SIEM User Management):** [View Screenshot](https://drive.google.com/file/d/1Kk5yyJEJ_DxJ36y_9y-SC74H1_NAlKRD/view?usp=sharing)

### **2️⃣ Set Up Elastic SIEM**
1. Sign up for an [Elastic SIEM Free Trial](https://www.elastic.co/security-labs/elastic-siem).
2. Deploy an **Elastic Cloud instance**.
3. Enable **security analytics** and configure log ingestion.

📸 **Hosts View in Elastic SIEM:** [View Screenshot](https://drive.google.com/file/d/1GQNUSHXbciwXyfIOuhZHj5qJTNDsGRI9/view?usp=sharing)

### **3️⃣ Install & Configure Elastic Defend Agent**
1. In **Elastic SIEM**, go to **"Fleet"** → **"Agents"**.
2. Click **"Add Agent"**, generate an installation script.
3. Run the script in PowerShell on the Windows VM.
4. Verify that logs are being ingested in **Elastic SIEM**.

📸 **Untitled Timeline in Elastic SIEM:** [View Screenshot](https://drive.google.com/file/d/1nDvQ1HoXrBRKuE0BsTSQ87HcYjm4hOwx/view?usp=sharing)

### **4️⃣ Simulate Malware Detection**
1. Download the [EICAR test file](https://www.eicar.org/?page_id=3950).
2. Attempt to execute it on the Windows VM.
3. Elastic Defend should detect and quarantine the file.
4. Review the alert in **Elastic SIEM** under the **Alerts tab**.

📸 **Event Details in Elastic SIEM:** [View Screenshot](https://drive.google.com/file/d/1dR21v0HYtuD5mQ5DWWBo9_lyF36v2inf/view?usp=sharing)

📸 **Alerts with Malware Prevention Alert Highlighted:** [View Screenshot](https://drive.google.com/file/d/179LcDVCNNbmTMTEfYh9yhzsQXrHj5XbQ/view?usp=sharing)

📸 **Endpoint Security Rule for Elastic Defend:** [View Screenshot](https://drive.google.com/file/d/15FSrPMJeq8mO9OeuS0rzIJWSZfkyD3ar/view?usp=sharing)

📸 **AWS EC2 Instance Monitoring:** [View Screenshot](https://drive.google.com/file/d/14IQWTfCx8gi2zyeRC-juscq9BKAlk2iB/view?usp=sharing)

📸 **AWS EC2 Resources Page:** [View Screenshot](https://drive.google.com/file/d/1g1P31RGXx-OKUkWze8xlT8v1uODjenaL/view?usp=sharing)

## 📊 Use Cases & Learning Outcomes
✅ Understand **SIEM architecture** and log ingestion  
✅ Gain hands-on experience in **malware detection & response**  
✅ Learn to configure **endpoint security agents**  
✅ Practice **SOC analyst workflows** with **alert analysis & triage**  

## 🔮 Future Enhancements
- 🛠 **Automate deployment** using Terraform
- 🔍 **Expand to Linux/macOS agents** for cross-platform monitoring
- 📈 **Create custom detection rules** in Elastic SIEM
- 🔒 **Integrate Splunk or other SIEM tools** for comparative analysis

## 🏆 Acknowledgments
Built as a hands-on cybersecurity project to simulate **real-world SOC workflows** and gain **practical experience** in threat detection & incident response. Inspired by **Elastic Security Labs** and AWS best practices.
