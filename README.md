### 📌 Scenario  
A junior developer accidentally published valid API keys in a public GitHub repository while testing a new feature.  
An external researcher discovered the exposed credentials and accessed real applicant data (names, emails, phone numbers, CV documents).  
The incident was responsibly disclosed, but represented a severe privacy and compliance violation.

### 🔍 Issues  
- Developer had unnecessary access to production API keys.  
- No automated detection for secrets in repositories.  
- Lack of strict role-based access and key segmentation.

### 📘 Review (NIST SP 800-53 AC-6)  
AC-6 enforces strict least-privilege access and recommends enhancements such as automated revocation, auditing, role-based access, and activity logging to prevent unauthorized exposure.

### 🛠 Recommendations  
- Enable automated **Secret Scanning / DLP** to detect leaked credentials.  
- Enforce **RBAC** to ensure developers only use non-production keys.  
- Implement **automatic key rotation** to invalidate exposed credentials quickly.

### 🎯 Outcome / Justification  
These controls would have prevented the exposure or drastically reduced the impact.  
Secret scanning detects leaked keys immediately, RBAC limits damage, and automated key rotation ensures short-lived credentials.

---
