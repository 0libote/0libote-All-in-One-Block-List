# 🛡️ 0libote All-in-One Blocklist

[![Stars](https://img.shields.io/github/stars/0libote/Pi-Hole-Blocklist?style=flat-square&logo=github&color=blue)](https://github.com/0libote/Pi-Hole-Blocklist/stargazers)
[![License](https://img.shields.io/github/license/0libote/Pi-Hole-Blocklist?style=flat-square&color=blue)](LICENSE)
![Domains Blocked](https://img.shields.io/badge/Domains~308,000-blue?style=flat-square)
![Last Updated](https://img.shields.io/badge/last%20updated-01%20August%202025-blue?style=flat-square)

---

A comprehensive, actively maintained DNS blocklist collection for **Pi-hole** and compatible DNS sinkholes. Blocks:

- Ads
- Trackers
- Telemetry
- Malware
- Phishing & scam domains

Designed for **high coverage with low false positives**. Ideal for home, office, and advanced users.

---

## 📦 Blocklists

### 🔹 All-in-One Blocklist  
Blocks ads, telemetry, trackers, malware, and more.

- **Domains:** ~308,000  
- **Link:**  
  ```
  https://raw.githubusercontent.com/0libote/Pi-Hole-Blocklist/main/All-in-One.txt
  ```

---

### 🔹 Trackers Only (Strict)  
Focused on tracking domains. May break services due to aggressive filtering.

- **Domains:** ~33,000  
- **Link:**  
  ```
  https://raw.githubusercontent.com/0libote/Pi-Hole-Blocklist/main/Trackers-Only.txt
  ```

---

### 🔹 Malware & Phishing  
Aggressively targets malicious domains.

- **Domains:** ~1,158,000  
- **Link:**  
  ```
  https://raw.githubusercontent.com/0libote/Pi-Hole-Blocklist/main/Malware-Phishing.txt
  ```

---

## ⚙️ How to Add to Pi-hole

1. Go to **Pi-hole Admin Panel**
2. Navigate to: `Group Management → Lists`
3. Paste the raw URL from the list above
4. Click **Add**
5. Go to `Tools → Update Gravity` to apply

---

## 🧱 What Is a DNS Sinkhole?

A **DNS sinkhole** blocks connections to unwanted or harmful domains at the DNS level.

### Benefits:
- 🌍 Network-wide blocking for all devices
- 🚫 Stops ads and trackers before they load
- 🛡️ Helps block malware/phishing domains
- 📵 Protects TVs, IoT, and mobile apps silently

> ⚠️ DNS filtering is a great **first line of defense** but should not replace antivirus or browser-based security tools.

---

## 🧪 How to Check What's Blocked

### Option 1: Web
- Open the list file in your browser and search (`CTRL+F`) for a domain

### Option 2: Terminal
```bash
pihole -q example.com
```
Shows whether the domain is blocked and by which list.

---

## 🚫 Troubleshooting

### Is a Site or App Broken?

This could be a **false positive**.

#### What to Do:
1. Check if the domain is blocked (`pihole -q`)
2. Temporarily whitelist via:
   ```
   pihole -w domain.com
   ```
3. Report it:
   [Open an issue](https://github.com/0libote/Pi-Hole-Blocklist/issues)

---

## 🔄 Updating the Blocklist

- Lists are updated regularly
- To update manually:
  - Go to Pi-hole → `Tools` → `Update Gravity`
- Or use a cron job to automate:
  ```bash
  pihole -g
  ```

---

## 💡 Best Practices

- ✅ Use **a few high-quality lists**
- ❌ Avoid mega-lists unless necessary
- 🔁 Update weekly
- 🧪 Test common services (e.g., streaming, banking)
- 👀 Review your logs for unexpected blocks

---

## 🙌 Contributing

You can help by:

- ⭐ Starring the repo
- 🐛 Reporting false positives
- 🔍 Suggesting domains to add/remove

---

## 🛠️ Upcoming Improvements

- More specific blocklists (e.g., NSFW, Gambling)
- Stricter all-in-one variant
- Automation via GitHub Actions

---

## 📚 Helpful Resources

- [Pi-hole Official Docs](https://docs.pi-hole.net/)
- [Pi-hole Discourse (Community)](https://discourse.pi-hole.net/)
- [Pi-hole GitHub](https://github.com/pi-hole/pi-hole)
- [Firebog Recommended Lists](https://firebog.net/)
- [avoidthehack - Blocklist Advice](https://avoidthehack.com/best-pihole-blocklists)

---

## 📜 License

MIT License — free for personal and commercial use.

> — Made with ❤️ by [0libote](https://github.com/0libote)
