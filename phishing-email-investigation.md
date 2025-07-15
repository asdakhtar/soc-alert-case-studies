### 📧 Alert Summary
- **Type**: Email Phishing  
- **Sender**: onboarding@hcronexx.thm  
- **Subject**: Action Required: Finalize Your Onboarding Profile  
- **Severity**: Medium  
- **Detection Source**: SOC Sim Lab – TryHackMe  

---

### 🧑‍💻 Investigation Steps
- Checked sender domain — `hcronexx.thm` not part of organization (`thetrydaily.thm`)
- Link led to a fake onboarding portal
- Used sandbox to confirm credential harvesting behavior
- Email header analysis showed spoofing (SPF fail, no DKIM)

---

### ✅ Final Verdict: Confirmed Phishing
> Credential harvesting attempt via fake onboarding page.  
> **Action taken**: Blocked sender domain, quarantined email, alerted users.

---

### 📘 Key Learnings
- Phishing tactics use urgency and impersonation  
- Link analysis and headers help confirm legitimacy  
- SOC triage helps prevent user compromise
