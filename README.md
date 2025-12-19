# 🔐 Data Leak: Least Privilege Failure  
**Focus:** Access Control · Data Protection · NIST SP 800-53

---

## 📌 Incident Summary
A data leak occurred when access to an internal folder containing **non-public product information, customer analytics, and promotional materials** was unintentionally shared outside the organization.

During an internal meeting, a sales manager granted team members access to a folder intended for internal use only. After the meeting concluded, access to the folder was **not revoked**. A warning was issued verbally, but no technical access controls were enforced.

Subsequently, a sales representative mistakenly shared a link to the internal folder with a business partner. The partner, believing the materials were approved for public distribution, posted the link on social media—resulting in unintended public exposure of internal data.
---

## 🚨 Primary Control Failure: Least Privilege
The core issue in this incident was a failure to properly enforce the **principle of least privilege**.

### Contributing Factors
- Access to sensitive information was broader than necessary  
- Permissions were not revoked after the meeting ended  
- Reliance on verbal guidance rather than technical controls  
- No automated or time-based access restrictions were in place

---

## 📖 NIST SP 800-53 Control Reference: AC-6
**AC-6 — Least Privilege** requires that users are granted **only the minimum level of access necessary** to perform their duties.

### Control Definition
Only the minimal access and authorization required to complete a task or function should be provided to users.

### Discussion
Access controls, user roles, and account permissions must be enforced to prevent users from operating at privilege levels higher than necessary. This reduces the risk of accidental or intentional misuse of sensitive information.

---

## 🛠️ Recommended Improvements

### 1️⃣ Restrict Access by Role
Only the sales manager should have retained access to the internal folder. Team members should have been granted **temporary, read-only access** during the meeting.

### 2️⃣ Automatically Revoke Access
Access to sensitive folders should be **automatically revoked** after a defined time period or meeting conclusion.

### 3️⃣ Enforce Technical Controls
Policies should be enforced through access management systems rather than relying on verbal warnings or manual processes.

### 4️⃣ Audit and Monitor Permissions
Regular audits of user access and activity logs should be conducted to ensure permissions remain appropriate over time.

---

## 🎯 Risk Reduction Impact
Implementing these controls would:
- Prevent accidental sharing of sensitive resources  
- Reduce exposure of non-public information  
- Minimize reliance on human memory and judgment  
- Align organizational practices with established security standards  

---

## 🎯 Key Skills Demonstrated
- Security incident analysis  
- Access control evaluation  
- Application of NIST SP 800-53  
- Least privilege enforcement strategies  
- Clear documentation of governance failures  

---

## 📚 Conclusion
This incident demonstrates how **non-malicious human error**, when combined with weak access controls, can result in significant data exposure. Enforcing least privilege through **technical safeguards, automated access revocation, and regular audits** would have prevented the leak entirely and reduced organizational risk.
