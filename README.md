<p align="center">
  <img src="./pxl.jpg" alt="Google Pixel Banner" width="600">
</p>


# 🔐 Critical Security Gap in Google Pixel 4a Battery Compensation Program

![Status](https://img.shields.io/badge/status-under%20review-yellow)
![Bug Type](https://img.shields.io/badge/type-security--bug-red)
![CVSS](https://img.shields.io/badge/CVSS-7.5--8.0-critical)
![License](https://img.shields.io/badge/license-MIT-blue)
![Last Update](https://img.shields.io/badge/last%20update-March%202025-brightgreen)
![Project](https://img.shields.io/badge/project-bug--report-orange)

---

## 🧾 Summary

This repository documents the discovery of a critical security vulnerability within Google's Pixel 4a battery replacement compensation process. The issue allows **non-eligible users** to claim compensation using **fake or generated IMEI numbers**, bypassing verification, and potentially causing **financial loss and identity fraud**.

---

## 👤 Reporter Information

- **Name:** Diva Lutfiando  
- **Email:** divaltfnd13@gmail.com  
- **Date of Analysis:** 15–20 March 2025  
- **Device Used:** Google Pixel 4a 4G *(original)* and Poco X6 5G *(testing)*  
- **Patch Version:** February 1, 2025  

---

## 🧪 Vulnerability Description

- Registering for compensation using **randomly generated IMEIs**
- Bypassing Google’s verification system
- Using non-Pixel devices and fake data to receive funds

---

## ⚙️ Proof of Concept (PoC)

### 🔗 Official URLs:
- [g.co/pixel/4abattery](https://g.co/pixel/4abattery)
- [Pixel Support Workflow](https://support.google.com/pixelphone/workflow/15642495)

### 🧪 Steps:

1. Open claim link and log in with any Gmail account  
2. Use IMEI generator ([imei.info](https://www.imei.info/imei-generator/))  
3. Paste IMEI in claim form  
4. Submit fake data  
5. System allows and approves application  
6. Multiple entries can be submitted using new data

### 🎥 [Video Proof](https://drive.google.com/file/d/10oYL0dQu_WuxrON4s7sDFkvb4BKTWzZX/view)

### 📸 Screenshot Evidence (some examples):
- [Battery Info](https://drive.google.com/file/d/1-n6gH-5tmeWsLpVmQ3i8Gmj9NlDwbD7M/view)
- [IMEI Submission](https://drive.google.com/file/d/10WSiljZYmnhUopk02H4FNgjfAeol1WwZ/view)
- [Verification Passed](https://drive.google.com/file/d/11CJWIes9I3Pyfvn6mgIbKa86RwFstjwr/view)

---

## 🔍 Vulnerability Metadata

| Key                | Value                                                      |
|--------------------|------------------------------------------------------------|
| **Bug ID**         | BatteryReplacement/UpdateSystemIncludeBugs                 |
| **Risk Level**     | High                                                       |
| **CVSS v3.1 Score**| 7.5–8.0                                                    |
| **Defect Types**   | User Fraud, Identity Exploit, Financial Misuse             |
| **Test Device**    | Poco X6 5G (non-Pixel device)                              |

---

## 🚨 Security Impact

1. **Unauthorized compensation claims**
2. **Potential financial abuse by third parties**
3. **Identity and IMEI ownership conflict**
4. **Compromise of device legitimacy check**
5. **Potential for scalable fraud using public tools**

---

## 🔒 Recommendations

1. **Verify IMEI via official device database**
2. **Account-to-device binding**
3. **Force screenshot/device-based validation**
4. **Restrict multiple claims per device/account**
5. **Routine audits of compensation system**

---

## 📝 Final Notes

This bug report was independently discovered and validated through multiple tests. The issue threatens both user safety and organizational trust if not addressed quickly.

> This repository aims to support Google in improving its device verification and anti-fraud mechanisms.

—

📁 [Full HTML report (local)](./SecurityGapIdentificationResults_Pxl4a.html)  
📁 [Follow-up Clarification Report](./ReportDetails_SecurityGap.html)

**Report by:**  
**Diva Lutfiando**  
_March 2025_

---

## 📄 License

This work is licensed under the [MIT License](LICENSE).

