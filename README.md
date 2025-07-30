# 🛡️ 0libote All-in-One Blocklist

[![Stars](https://img.shields.io/github/stars/0libote/0libote-All-in-One-Block-List?style=flat-square&logo=github&color=blue)](https://github.com/0libote/0libote-All-in-One-Block-List/stargazers)
[![License](https://img.shields.io/github/license/0libote/0libote-All-in-One-Block-List?style=flat-square&color=blue)](LICENSE)
![Last Updated](https://img.shields.io/badge/last%20updated-28%20July%202025-blue?style=flat-square)
![Domains Blocked](https://img.shields.io/badge/domains%20blocked-~1,749,000-blue?style=flat-square)

---

A comprehensive, community-driven DNS blocklist for **Pi-hole** and other DNS sinkhole tools. It blocks ads, trackers, telemetry, malware, phishing, and scam domains — with a focus on high coverage and low false positives. Perfect for both beginners and power users.

---

## 📑 Table of Contents

- [📦 Blocklist Overview](#-blocklist-overview)
- [🧱 Included Lists](#-included-lists)
- [📘 What Is a DNS Sinkhole?](#-what-is-a-dns-sinkhole)
- [⚙️ How to set up](#-how-to-use-this-with-pi-hole)
- [🔍 How to Check Blocked Domains](#-how-to-check-blocked-domains)
- [⚠️ Troubleshooting & False Positives](#️-troubleshooting--false-positives)
- [🔄 Updating the Blocklist](#-updating-the-blocklist)
- [💡 Best Practices](#-best-practices)
- [🙌 Contributing](#-contributing)
- [📜 License](#-license)

---

## 📦 Blocklist Overview

- **Name:** 0libote All-in-One Blocklist  
- **Total Domains Blocked:** ~1,749,000  
- **Last Updated:** 28 July 2025  

This single master list aggregates multiple curated lists to create a strong, balanced solution with minimal false positives.

---

## 🧱 Included Lists

All the domain entries from the lists below are **included in the All-in-One Blocklist**.

| List | Description | Link |
|------|-------------|------|
| **Trackers** | Blocks analytics and tracking beacons | [Trackers.txt](https://raw.githubusercontent.com/0libote/0libote-All-in-One-Block-List/refs/heads/main/Tracker%20Only%20Blocklist.txt) |
| **Malware & Phishing** | Known malicious domains, ransomware C2s, and phishing sites | [Malware-Phishing.txt](https://raw.githubusercontent.com/0libote/0libote-All-in-One-Block-List/refs/heads/main/Malware%20%26%20Phishing%20Only%20Blocklist.txt) |


> All domains from these files are merged into [Blocklist.txt](https://github.com/0libote/0libote-All-in-One-Block-List/blob/main/Blocklist.txt).

---

## 📘 What Is a DNS Sinkhole?

A **DNS sinkhole** intercepts DNS queries to unwanted or malicious domains and blocks them before they reach your device.

### ✅ Why Use One?

- 🚫 Blocks ads and trackers network-wide
- 🛡️ Stops access to malware and phishing servers
- 🕵️ Blocks telemetry and data collection at the source
- 👪 Protects **every device** on your network — phones, TVs, and more

> ⚠️ **Note:** A DNS sinkhole is a powerful layer of protection, but not a full antivirus replacement. Always stay cautious online.

---

## ⚙️ How to Use This with Pi-hole

1. Access your Pi-hole admin dashboard: `http://pi.hole/admin`
2. Go to **Group Management** → **Adlists**
3. Paste this URL into the **Address** field:

   ```
   https://raw.githubusercontent.com/0libote/0libote-All-in-One-Block-List/refs/heads/main/Blocklist.txt
   ```

4. Click **Add**
5. Go to **Tools** → **Update Gravity**

Your Pi-hole will now use the full All-in-One blocklist.

---

## 🔍 How to Check Blocked Domains

### 🌐 Option 1: Search the File

- Open the [Blocklist File](https://raw.githubusercontent.com/0libote/0libote-All-in-One-Block-List/refs/heads/main/Blocklist.txt)
- Press `CTRL+F` / `CMD+F` and search for a domain like `example.com`

### 💻 Option 2: Terminal Query

```bash
pihole -q domain.com
```

Replace `domain.com` with the address you want to check. It will show if and where it's blocked.

---

## ⚠️ Troubleshooting & False Positives

### A Site or App Doesn't Work?

This may be caused by a **false positive**.

### How to Fix or Report:

1. Confirm the domain is in the blocklist (see above)
2. [Open an Issue](https://github.com/0libote/0libote-All-in-One-Block-List/issues)
3. Provide:
   - The domain
   - Description of the problem (e.g. "banking app broken")

We'll investigate and adjust accordingly.

---

## 🔄 Updating the Blocklist

- ✅ The list is **updated frequently** to include new threats and remove false positives
- 🔁 Manual update:
  - Go to **Tools** → **Update Gravity** in the Pi-hole dashboard

---

## 💡 Best Practices

- ✅ Stick with **a few high-quality lists** to reduce false positives
- ❌ Avoid bloated "mega lists" unless necessary
- 🔄 Update blocklists weekly or automate with cron
- 🧪 Test services like banking, streaming, and email for blocking issues
- 🧠 Don’t rely solely on DNS filtering — practice good security habits

---

## 🙌 Contributing

You can help improve this list:

- ⭐ Star the repository to show support  
- 🐞 [Report issues or false positives](https://github.com/0libote/0libote-All-in-One-Block-List/issues)  
- 📬 Suggest useful domains (or removals) via GitHub Issues or PRs  
- 🔍 Help audit false positives

---

## 📜 License

Licensed under the [MIT License](LICENSE).  
Free for personal, educational, and commercial use.

---

> — Made with ❤️ by [0libote](https://github.com/0libote)