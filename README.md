![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)

[![Pi-hole Generation](https://github.com/madnesscc/adguard-allowlist-cloudgaming/actions/workflows/generate_pihole_cloud.yml/badge.svg)](https://github.com/madnesscc/adguard-allowlist-cloudgaming/actions/workflows/generate_pihole_cloud.yml)

# 🎮 AdGuard Whitelist for Cloud Gaming

Optimize your Cloud Gaming experience (Amazon Luna, Xbox Cloud Gaming, NVIDIA GeForce Now) while using AdGuard, uBlock Origin, or other adblockers.

## Cloudgaming Allowlist

This list ensures that cloud gaming services like GeForce Now, Xbox Cloud, and Luna run smoothly without being blocked by DNS filters.

### 📥 Download & Installation

| Platform | Filter Type | Link |
| :--- | :--- | :--- |
| **AdGuard / uBlock** | Standard (Allowlist) | [adguard-allowlist-cloudgaming](./adguard-allowlist-cloudgaming) |
| **Pi-hole / DNS** | Clean Domains | [pihole-cloudgaming.txt](./pihole-cloudgaming.txt) |

> **Status:** The Pi-hole version is automatically generated and updated on every change.

## ❓ Why do you need this list?
Aggressive adblocking filters and privacy settings can sometimes accidentally block essential STUN servers and WebRTC connections. If your adblocker interferes with these domains, you might experience:
- Infinite loading screens or failed handshakes
- High input lag and stuttering streams
- "Network Error" messages when trying to launch a game (especially in fast-paced shooters like Fortnite)

This whitelist uses the `$important` modifier to ensure that crucial infrastructure and video streaming domains are completely bypassed by your adblocker. This guarantees minimum latency and a stable connection.

## 🚀 How to use

**Method 1: Copy & Paste**
1. Open your **AdGuard Settings**.
2. Navigate to **User Rules** (or Custom Filters).
3. Open the `whitelist.txt` file from this repository, copy its entire content, and paste it into the text box.
4. Save and apply! 

*(Note: This syntax also works for uBlock Origin in the "My filters" tab.)*

**Method 2: Import as a Filter List (AdGuard)**
1. Go to **Filters** -> **Custom Filters** -> **Add Custom Filter**.
2. Paste the raw URL of the `whitelist.txt` file from this repository.
3. AdGuard will now automatically keep the list updated if new servers are added here!

## 💡 Extra Tips for Best Performance
- **Disable "Block WebRTC":** If you are using AdGuard's Stealth Mode or Tracking Protection in your browser, make sure the option to block WebRTC is **disabled**. Cloud gaming heavily relies on WebRTC.
- **Use a fast DNS:** For the best gaming experience, consider using a fast upstream DNS server like Cloudflare (`1.1.1.1`) or Google (`8.8.8.8`).
---
**Disclaimer:** This project is not affiliated with Amazon, NVIDIA, Microsoft, Google, or any other cloud gaming provider. All product names, logos, and brands are property of their respective owners. This list is maintained by **madnesscc** for community use under the MIT License.
