# RG AutoMod – Discord Link Moderation Bot

RG AutoMod is a simple and efficient moderation bot designed to automatically block unwanted links in Discord servers.  
It provides link protection, trusted-user controls, custom whitelists, logging, and optional strike-based punishment.  
This repository contains full documentation. The bot's source code is private and licensed.

---

## Invite the Bot
Official bot invite URL:
https://invite-rgautomod.rixstongamer.xyz

---

## Overview
RG AutoMod scans messages in real time and removes any links posted by users who are not trusted, not whitelisted, or not in allowed channels.

Main capabilities:
- Automatic link detection and removal  
- Trusted user system (temporary & permanent)  
- Channel allowlist system  
- Default safe whitelist  
- Custom whitelist patterns  
- Optional auto-punishment  
- Logging system  
- Custom warning messages  
- Persistent storage  
- Auto welcome/setup message  
- Dynamic status updates  

---

## Features

### 1. Automatic Link Blocking
- Detects http/https links, “www.” links, and raw domain names  
- Supports all major domain extensions  
- Removes messages instantly  
- Sends a temporary warning (auto-deletes after 5s)  

---

### 2. Default Whitelisted Links
Some important and safe links are allowed by default, such as:
- rixstongamer.xyz  
- rixxymc.in  
- Official YouTube channels  
- Official Instagram  

These links cannot be removed.

---

### 3. Trusted User System
**Permanent trust:**  
/trust-user @user  

**Temporary trust:**  
/trust-user @user 1h  
/trust-user @user 30m  
/trust-user @user 2d  

**Management:**  
/untrust-user @user  
/list-trusted  

---

### 4. Channel Allowlist
Allow specific channels to use links:

/allow-channel #channel  
/block-channel #channel  
/list-channels  

---

### 5. Custom Whitelist
Add your own allowed links or patterns:

/add-whitelist pattern  
/remove-whitelist pattern  
/list-whitelist  
/reset-whitelist  

Examples:
- /add-whitelist discord.gg  
- /add-whitelist twitter.com  

---

### 6. Link Logging
Enable a log channel to track deleted links:

/set-log-channel #channel  
/remove-log-channel  

Logs show:
- User  
- Channel  
- Message  
- Strike count  
- Timestamp  

---

### 7. Custom Warning Messages
/set-warning message  
/reset-warning  

---

### 8. Auto-Punishment (Optional)
/punishment enable  
/punishment disable  
/punishment-config [max_strikes] [timeout_minutes]  
/reset-strikes @user  

Default:
- 3 strikes  
- 10-minute timeout  

---

### 9. Persistent Storage
The bot automatically saves:
- Trusted users  
- Temporary trust timers  
- Allowed channels  
- Custom whitelists  
- Warning settings  
- Log channel settings  
- Punishment settings  
- Strike counts  

---

### 10. Dynamic Status
Updates automatically, for example:
“Watching 12 servers | /help”

---

### 11. Welcome Message
When the bot joins a server, it posts:
- Setup instructions  
- Safe link list  
- Basic help info  

---

## Documentation

Complete docs are available in the /docs folder:

- docs/overview.md  
- docs/features.md  
- docs/commands.md  
- docs/setup.md  
- docs/permissions.md  
- docs/changelog.md  
- docs/support.md  

---

## License
RG AutoMod is a proprietary, closed-source project.  
Code redistribution or modification is not allowed.  
Documentation may be viewed publicly.

---

## Support
Support server:  
https://dsc.gg/rixstongamer

Created by RixStonGamer
