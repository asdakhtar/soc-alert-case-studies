### 🌍 Alert Summary
- **Type**: Blocked Outbound URL  
- **Source IP**: 10.20.2.17  
- **Destination IP**: 67.199.248.11  
- **Destination Port**: 80  
- **URL**: http://bit.ly/3sHkX3da12340  
- **Detection Source**: Firewall (web-browsing app)  
- **Rule Triggered**: Blocked Websites  
- **Action**: Blocked

---

### 🔍 Indicators of Attack
- Shortened link used to mask external malicious destination  
- Destination IP flagged in threat intel feeds  
- Web-browsing activity indicates user-initiated access

---

### 🧑‍💻 Investigation Workflow
- Mapped Source IP to internal user  
- Expanded Bitly link using sandbox (e.g., urlscan.io)  
- Ran threat intel scans (AlienVault, Hybrid Analysis)  
- Compared against other logs for repeated attempts

---

### ✅ Final Verdict: True Positive – Blocked Threat
> Attempted access to malicious domain blocked by firewall.  
> **Action taken**: Notified user, reviewed endpoint, reinforced training on shortened links.

---

### 📘 Key Learnings
- Firewalls play crucial role in blocking outbound threats  
- SOC teams must follow up on “blocked” alerts to confirm intent  
- URL expansion and IP analysis are core investigation tools
