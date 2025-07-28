# 🛡️ 0libote All-in-One Blocklist

A powerful, blocklist designed for **Pi-hole** and other DNS Sinkhole users who want comprehensive blocking of ads, trackers, telemetry, malware, phishing and other unwanted domains. This works as a **all in one list** trying to create a list that covers all for beginners while having as little false positives as possible.

---

## 📦 About This Blocklist

- **List Name:** 0libote All-in-One Blocklist
- **Total Domains Blocked:** ~1,757,000
- **Last Updated:** 28 July 2025

---

## 📘 What is a DNS Sinkhole?

A **DNS sinkhole** intercepts DNS queries for unwanted or malicious domains and redirects them so they **never reach your devices**. Tools like **Pi-hole** replace your network's default DNS to achieve this.

### ✅ Benefits of a DNS Sinkhole

- 🚫 Helps to block ads **across your whole network** — no browser extensions needed
- 🛡️ Helps to protect against malware, phishing, and scams
- 🕵️ Helps to stop tracking and telemetry services
- 👪 Centralized protection for **all devices** instead of the typical per device protection 

> 💡 **Note:** Once Pi-hole or another DNS Sinkhole is set as your DNS server, all devices using that network are automatically protected. A DNS Sinkhole is not a perfect bulletproof protection against adverts, malware and other items however it is a good start. Always remain vigilant when surfing the web, Bad actors are always trying to exploit you.

---

## 📄 How to Use This Blocklist with Pi-hole

### Step-by-step Setup

1. Log in to your Pi-hole dashboard (`http://pi.hole/admin`).
2. Navigate to **Group Management** → **Adlists**.
3. Paste this blocklist URL in the **Address** field:

   ```
   https://raw.githubusercontent.com/0libote/0libote-All-in-One-Block-List/refs/heads/main/Blocklist.txt
   ```

4. Click **Add**.
5. Go to **Tools** → **Update Gravity**, then click **Update**.

Your Pi-hole will now start filtering domains using this blocklist.

---

## 🔎 How to Check if a Domain is Blocked

### 🔍 Option 1: Using a Web Browser

1. Open the [Blocklist File](https://raw.githubusercontent.com/0libote/0libote-All-in-One-Block-List/refs/heads/main/Blocklist.txt)
2. Press `CTRL+F` (or `CMD+F` on Mac) to search for a domain like `example.com`

If it appears in the list, it’s being blocked.

---

### 💻 Option 2: Using the Terminal (Check All Lists in Pi-hole)

To check if a domain is being blocked by **any** list in your Pi-hole:

```bash
pihole -q domain.com
```

Replace `domain.com` with the domain you're checking.  
This will show which blocklist (if any) is blocking the domain.

---

## ⚠️ Troubleshooting & False Positives

### Problem: A site or app is not working
It could be a **false positive** (a good domain mistakenly blocked).

### Steps to Fix:

1. Confirm the domain is on this blocklist (see section above).
2. Open a [GitHub Issue](https://github.com/0libote/0libote-All-in-One-Block-List/issues).
3. Include:
   - The **domain name**
   - A short explanation 

---

## 🔄 Updating the Blocklist

- ✅ This blocklist is updated regularly with new domains and to fix possible false positive. If you find any false positives or key missing domains feel free to let us know so we can add or remove them ASAP.
- 🔁 To update Pi-hole:
  - Go to **Tools** → **Update Gravity**

---

## 🛠️ Tips & Tools for Beginners

### Useful Tools

- **[Pi-hole Documentation](https://docs.pi-hole.net)** – Details about Pi-hole
- **[dnsleaktest.com](https://dnsleaktest.com/)** – Confirm DNS is routing through DNS Sinkhole

---

## 💡 Best Practices

- ✔️ Use **only a few high-quality blocklists** to reduce false positives.
- ❌ Don’t overblock — more isn’t always better.
- 🧪 Periodically check important services (like banking, email) for issues.
- 🔄 Keep Pi-hole and blocklists updated.

---

## 🙌 How to Contribute

Ways to help:

- ⭐ Star the repo to support the project
- 🐞 [Report issues](https://github.com/0libote/0libote-All-in-One-Block-List/issues)
- ✅ Submit issues to help improve the list

---

## 📜 License

Licensed under the [MIT License](LICENSE).  
Free for personal, educational, or commercial use.

---

> — Made with ❤️ by **0libote**
