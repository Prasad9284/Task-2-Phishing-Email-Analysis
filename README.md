# Task-2-Phishing-Email-Analysis
# 🛡️ Phishing Email Analysis – Cyber Security Internship

## 📌 Objective
To analyze a suspicious email and identify phishing characteristics such as spoofed sender addresses, suspicious links, urgent language, and other red flags.

---

## 🛠 Tools Used
- **Proofpoint Threat Reference** (Sample phishing email source)
- **MXToolbox / Google Header Analyzer** (Optional – for header analysis)
- Web browser (for link inspection without clicking)

---

## 🖥 Steps Performed

### **1. Obtained a Sample Phishing Email**
- Sample taken from Proofpoint: [Phishing Email Example](https://www.proofpoint.com/us/threat-reference/phishing)
- Screenshot saved as `screenshots/01-phishing-email.png`

---

### **2. Examined Sender's Email Address**
- **From:** `GlobalPayVYT@globalpay.com`
- Indicators of spoofing:
  - Extra characters in the username (`VYT`).
  - Domain name could be impersonating a legitimate payment service.
  - Not matching the email formatting style of official companies.

---

### **3. Checked Email Headers (Optional)**
- Email headers can be analyzed using:
  - [Google Header Analyzer](https://toolbox.googleapps.com/apps/messageheader/)
  - [MXToolbox](https://mxtoolbox.com/EmailHeaders.aspx)
- In real cases, mismatch between `Return-Path` and `From` confirms spoofing.

---

### **4. Identified Suspicious Links/Attachments**
- Contains HTML attachment: `update2816.html (7 KB)`
- HTML files in phishing emails often contain credential-stealing forms or redirect to malicious sites.

---

### **5. Detected Urgent/Threatening Language**
- Text: *“Your account has been restricted”*
- Purpose: Create panic and force user to click link or open attachment.

---

### **6. Checked for Grammar/Spelling Issues**
- The tone and structure do not match professional communication.
- Generic greeting (“Dear customer”) instead of personalized address.

---

### **7. Summary of Phishing Traits Found**
- Spoofed sender address.
- Unnecessary attachment (HTML).
- Urgent language to scare the user.
- Generic greeting.
- Risk of credential theft.

---

## 📊 Final Analysis Table

| Indicator Type         | Example from Email                                  | Risk Level |
|------------------------|-----------------------------------------------------|------------|
| **Spoofed Sender**     | `GlobalPayVYT@globalpay.com`                         | High       |
| **Suspicious File**    | `update2816.html`                                   | High       |
| **Urgent Language**    | “Your account has been restricted”                   | Medium     |
| **Generic Greeting**   | “Dear customer”                                      | Medium     |
| **Link/Attachment**    | Unknown link in HTML file                            | High       |

---

## 📸 Screenshots
- **1. Sample Phishing Email**  
  ![Phishing Email](screenshots/01-phishing-email.png)

---

## 🛡 Recommendations
- Never click on links or download attachments from unknown senders.
- Verify sender’s domain and email headers.
- Use a spam filter and keep it updated.
- Educate users to identify phishing traits.

---

## 📂 Repository Structure
📁 phishing-email-analysis
├── README.md
├── screenshots/
│ └── 01-phishing-email.png
└── phishing_analysis.txt # Optional plain text report


---

## 📎 References
- [Proofpoint Threat Reference – Phishing](https://www.proofpoint.com/us/threat-reference/phishing)
- [Google Header Analyzer](https://toolbox.googleapps.com/apps/messageheader/)
- [MXToolbox](https://mxtoolbox.com/EmailHeaders.aspx)

