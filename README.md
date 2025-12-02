# ⚡ Cybersecurity Daily Drills

![Focus](https://img.shields.io/badge/Focus-Skill_Building-orange?style=for-the-badge&logo=muscle&logoColor=white)
![Language](https://img.shields.io/badge/Language-Bash_%7C_Python-yellow?style=for-the-badge&logo=gnu-bash&logoColor=white)
![Status](https://img.shields.io/badge/Status-Active_Learning-success?style=for-the-badge)

## 📖 The Training Ground
Welcome to my digital workbench. While my [Cybersecurity Portfolio](https://github.com/d-osei/Cybersecurity-Portfolio) hosts polished, end-to-end investigations, this repository is for **repetition, experimentation, and muscle memory.**

Here is where I document the daily tasks required to master the **Art of Investigation**, from Linux administration to SOC incident response workflows.

---

## 📂 Repository Contents

### 🐧 [Linux Operations](/Linux_Ops)
*Scripts and reference guides for system administration.*
* **User Management:** Scripts for onboarding/offboarding and permission audits (`chmod`/`chown`).
* **Hardening:** Basic firewall (`ufw`) setups and SSH configuration notes.
* **Log Review:** Command cheat sheets for parsing `auth.log` and `syslog`.

### 📘 [SOC Playbooks](/SOC_Playbooks)
*Standard Operating Procedures (SOPs) for Tier 1 & 2 Analysis.*
* **Phishing Triage:** Step-by-step analysis of suspicious emails.
* **Malware Isolation:** Procedures for containing infected hosts.
* **Account Compromise:** Incident response flow for compromised credentials.

### 🧪 [Lab Journal](/Lab_Journal)
*Raw notes and "Quick Wins" from the home lab.*
* Configuration snippets for **Splunk** inputs.
* Troubleshooting notes for **VMware ESXi** networking.
* Quick Python scripts for data manipulation.

---

## 🛠️ "Code-First" Learning

I believe in automating the boring stuff. You will find many "One-Liner" scripts here designed to speed up analysis.

**Example: Quick IP Extraction**

This command pulls IP addresses from a log file, counts the frequency of each IP, and sorts them to show the "noisiest" talkers first.

```bash
grep -oE "\b([0-9]{1,3}\.){3}[0-9]{1,3}\b" access.log | sort | uniq -c | sort -nr
```
**Breakdown of the Command:**

* `grep -oE "..."`: Searches the file.

  * `-o`: **Only** output the matching text (the IP), not the whole line.

  * `-E`: Use **Extended** Regex (allows us to use special patterns).

  * `\b([0-9]{1,3}\.){3}[0-9]{1,3}\b`: The Regex pattern for an IPv4 address (four groups of numbers separated by dots).

* `|`: The Pipe. Passes the output of the previous command to the next one.

* `sort`: Groups similar lines together (required before using `uniq`).

* `uniq -c`: Removes duplicates but counts (`-c`) how many times each IP appeared.

* `sort -nr`: Sorts the final list.

  * `-n`: Sort **Numerically** (by the count).

  * `-r`: **Reverse** order (biggest numbers at the top).

---
