# 🛡️ 0libote All-in-One Blocklist

  

[![Stars](https://img.shields.io/github/stars/0libote/0libote-All-in-One-Block-List?style=flat-square&logo=github&color=blue)](https://github.com/0libote/0libote-All-in-One-Block-List/stargazers)
[![License](https://img.shields.io/github/license/0libote/0libote-All-in-One-Block-List?style=flat-square&color=blue)](LICENSE)
![Last Updated](https://img.shields.io/badge/last%20updated-28%20July%202025-blue?style=flat-square)
  
---

  

A comprehensive DNS blocklist for **Pi-hole** and other DNS sinkhole tools. Blocks ads, trackers, telemetry, malware, phishing, and scam domains with a focus on high coverage and low false positives. Perfect for both beginners and more experienced users.

  

---

  

## 📑 Table of Contents

  
- [📦 Blocklist Overview](#-blocklist-overview)
- [🧱 Included Lists](#-included-lists)
- [📘 What Is a DNS Sinkhole?](#-what-is-a-dns-sinkhole)
- [🔍 How to Check Blocked Domains](#-how-to-check-blocked-domains)
- [⚠️ Troubleshooting & False Positives](#️-troubleshooting--false-positives)
- [🔄 Updating the Blocklist](#-updating-the-blocklist)
- [💡 Best Practices](#-best-practices)
- [🙌 Contributing](#-contributing)
- [📜 License](#-license)

---


## 📦 Blocklist Overview

## 0libote All-in-One Blocklist  
- **Last Updated:** 1 August 2025  

## All in one 
**Info:** Intended to be a all in one blocklist. Blocking a bit of everything with minimal false positives.
**Domains blocked:** ~307,000

**Link:** 
```
https://raw.githubusercontent.com/0libote/Pi-Hole-Blocklist/refs/heads/main/Blocklist.txt
```

## Tracker only
**Info:** A more strict list focusing only on blocking trackers. Higher chance of false positives as not maintained as much. 
**Domains blocked:** ~33,000

**Link:** 
```
https://github.com/0libote/Pi-Hole-Blocklist/blob/main/Tracker%20Only%20Blocklist.txt`
```

## Malware & Phishing only 
**Info:** A large blocklist including many many domains affiliated with possible malware and phishing attempts. Also includes other malicious sites.
**Domains blocked:** ~1,157,000

**Link:** 
```
https://raw.githubusercontent.com/0libote/Pi-Hole-Blocklist/refs/heads/main/Malware%20%26%20Phishing%20Only%20Blocklist.txt
```

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

**In progress**
- More lists that are more specific (e.g NSFW/gambling Block)
- More work on the README
- More strict all in one list
- Much more 😉

---

  

## 📜 License

Licensed under the [MIT License](LICENSE).  
Free for personal, educational, and commercial use

---

  

> — Made with ❤️ by [0libote](https://github.com/0libote)