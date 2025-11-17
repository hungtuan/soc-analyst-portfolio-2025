# 🛡️ SOC Analyst Portfolio – 2025

**Author:** Hung Tuan  
**Role Target:** SOC Analyst Intern / Blue Team / Security Analyst Tier 1  
**Tools:** Splunk, ELK Stack, Microsoft Sentinel, Wireshark

---

## 🚀 Giới thiệu

Đây là portfolio tổng hợp các bài phân tích sự kiện bảo mật, lab thực hành SIEM, detection rule và playbook điều tra sự cố.  
Mục tiêu của portfolio này là chứng minh khả năng:

- Đọc & phân tích log trên SIEM (Splunk, ELK, Sentinel)
- Xác định hành vi bất thường (4625, brute force, SSH fail…)
- Viết detection rules (SPL, KQL, Elastic DSL)
- Thực hiện điều tra SOC Tier 1
- Xây dựng playbook xử lý sự cố theo chuẩn NIST

Portfolio được cập nhật liên tục trong năm 2025.

---

# 📂 Danh mục nội dung

## 1️⃣ **Case Reports (Điều tra sự cố)**

> Các phân tích log Windows, Linux, Web và hành vi tấn công.

- **[Windows 4625 – Failed Logon Analysis](case-reports/windows-4625-analysis.md)**
- **[Windows 4624 – Successful Logon Analysis](case-reports/windows-4624-success-login.md)**
- **[Windows 4672 – Admin Privilege Granted](case-reports/windows-4672-admin-privilege.md)**
- **[Linux auth.log – SSH Failed Login Case](case-reports/linux-authlog-ssh-failed.md)**
- **[Brute Force RDP Case Study](case-reports/brute-force-rdp-case.md)**
- **[Web Access Log Attack Analysis](case-reports/web-accesslog-attack-analysis.md)**

---

## 2️⃣ **SIEM Queries (Detection Rules)**

### 🔹 Splunk (SPL)

- [Brute Force Detection Rule](siem-queries/splunk/brute_force_detection.spl)
- [Failed Login Count](siem-queries/splunk/failed_login_count.spl)

### 🔹 Microsoft Sentinel (KQL)

- [Brute Force Rule](siem-queries/sentinel/brute_force_detection.kql)
- [Suspicious Login Rule](siem-queries/sentinel/suspicious_login.kql)

### 🔹 Elastic (DSL)

- [SSH Brute Force Detection](siem-queries/elk/ssh_bruteforce.dsl)

---

## 3️⃣ **Playbooks (SOC Tier 1)**

- **[4625 Investigation Playbook](playbooks/4625_investigation_playbook.md)**
- **[Brute Force RDP Playbook](playbooks/brute_force_rdp_playbook.md)**
- **[SSH Brute Force Response](playbooks/ssh_brute_force_playbook.md)**
- **[Privilege Escalation Playbook](playbooks/privilege_escalation_playbook.md)**

---

## 4️⃣ **Notes (Kiến thức tổng hợp)**

- **[EventID Cheat Sheet](notes/eventid_cheatsheet.md)**
- **[Windows Logon Types](notes/windows_logon_types.md)**
- **[SOC Tier 1 Checklist](notes/soc_tier1_checklist.md)**
- **[SIEM Basics](notes/siem_basics.md)**

---

## 5️⃣ **Screenshots (Lab Evidence)**

> Ảnh chứng minh em đã thực hành lab thật trên Splunk/ELK/Sentinel.

- Splunk 4625
- Splunk 4624
- SSH Fail logs
- RDP brute force timeline

---

# 🎯 Mục tiêu nghề nghiệp

Tìm kiếm cơ hội **Thực tập SOC Analyst / Blue Team** để áp dụng các kỹ năng:

- Log analysis
- Alert triage
- Investigation
- Incident Response
- Threat detection

---

# 📧 Liên hệ

---

_Cảm ơn anh/chị đã dành thời gian xem portfolio của em!_
