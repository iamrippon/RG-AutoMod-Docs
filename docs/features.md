# ✨ RG AutoMod — Full Feature Documentation

RG AutoMod is a complete, high-performance link moderation system designed to protect Discord communities from unwanted links, spam, scams, and unauthorized promotions.  
This document provides a full technical breakdown of every feature included in the bot.

---

# 1. 🔗 Automatic Link Detection & Removal

RG AutoMod instantly detects and removes unwanted links in real time.

### ✔ Detects:
- http:// and https:// links  
- www. links  
- Raw domains (example.com)  
- All major TLDs (.com, .net, .org, .gg, .xyz, .io, etc.)

### ✔ How it works:
1. A user sends a message containing a link  
2. Bot deletes it instantly  
3. A temporary warning is shown (auto-deletes after 5s)  
4. (Optional) Logged in the log channel  

### ✔ Warning message features:
- Auto-deletes  
- Customizable by admins  

---

# 2. 🔒 Default Whitelist System

These are safe, pre-approved links that are **always allowed**:

### ✔ Important Default Links (short list)
- rixstongamer.xyz  
- rixxymc.in  
- youtube.com/@RixStonGamer  
- instagram.com/rixstongamer  

### Key features:
- Case-insensitive  
- Supports http / https / no prefix  
- Cannot be removed (protected)  

---

# 3. 👤 User Trust System

Trusted users can bypass link blocking.

## 🔹 Permanent Trust
/trust-user @user

- User may post links in all channels  
- Does not expire  
- Saved through bot restarts  

## 🔹 Temporary Trust


/trust-user @user 1h


Supported formats:
- 15s  
- 30m  
- 1h  
- 2d  

Auto-expires once the timer ends.

## 🔹 Manage Trust


/untrust-user @user
/list-trusted


---

# 4. 📺 Channel Allowlist

Admins can choose which channels allow links.

### Commands:


/allow-channel #channel
/block-channel #channel
/list-channels


### Examples:
- Allow links in #media  
- Allow promotions in #ads  
- Block links everywhere else  

---

# 5. ✅ Custom Whitelist System

Admins can add or remove allowed links for their server.

### Commands:


/add-whitelist pattern
/remove-whitelist pattern
/list-whitelist
/reset-whitelist


### Examples:
/add-whitelist discord.gg  
/add-whitelist twitter.com  
/add-whitelist example.com/promo  

Supports:
- Partial match  
- Case-insensitive  
- Specific URLs or full domains  

---

# 6. 📊 Link Deletion Logging

Log every deleted link to a chosen channel.

### Commands:


/set-log-channel #channel
/remove-log-channel


### Log entry includes:
- User  
- Channel  
- Message content  
- Timestamp  
- Strike count (if punishment is enabled)  

Example:


🔗 Link Deleted
User: @John
Channel: #general
Message: "Check this out: example.com"
Strike: 1/3
Time: 2:30 PM


---

# 7. 💬 Custom Warning Messages

Customize the warning message shown when a link is blocked.

### Commands:


/set-warning message
/reset-warning


Example:


/set-warning Links are restricted! Please check #rules.


---

# 8. ⚖️ Auto-Punishment System (Optional)

Progressive punishment for repeated violations.

### Enable / Disable:


/punishment enable
/punishment disable


### Configure:


/punishment-config [max_strikes] [timeout_minutes]


### Default:
- 3 strikes  
- 10-minute timeout  

### Behavior:
- Strike 1 → warning  
- Strike 2 → warning  
- Strike 3 → timeout  
- Strikes reset after timeout  

### Manual reset:


/reset-strikes @user


---

# 9. 💾 Persistent Storage

Everything is saved into a JSON storage file:

- Trusted users  
- Temporary trust timers  
- Allowed channels  
- Custom whitelist  
- Logging settings  
- Punishment settings  
- Strike counts  
- Custom warning message  

Reloads automatically on startup.

---

# 10. 🔄 Dynamic Bot Status

Updates every 30 seconds with:
- Total servers  
- /help command hint  

Example:


Watching 12 servers | /help


---

# 11. 👋 Welcome Message

When added to a server, the bot automatically sends:

- Quick setup instructions  
- Default safe links  
- /help usage info  
- Support link  

---

# 12. 📈 Full Statistics Dashboard (/status)

Shows:

### 🌐 Global:
- Total servers  
- Total users  
- Bot latency  

### 📊 Server:
- Trusted users  
- Temporary trusted users  
- Allowed channels  
- Whitelisted patterns  
- Logging status  

### ⚙️ Configuration:
- Punishment enabled/disabled  
- Max strikes  
- Timeout duration  
- Custom warning  

---

# 13. 🎯 Permission System

### Who is allowed to post links?

| User Type        | Allowed |
|-----------------|---------|
| Admins          | ✔ Always |
| Trusted Users   | ✔ |
| Allowed Channels| ✔ |
| Whitelisted Links | ✔ |
| Normal Users    | ❌ |

### Priority Order:
Admin > Allowed Channel > Trusted User > Whitelisted Link > Block  

---

# 14. 🎨 Bot Behavior

### Bot ignores:
- Admins  
- Other bots  
- Itself  
- Whitelisted links  
- Trusted users  
- Allowed channels  

### Bot blocks:
- All other link attempts  
- Unapproved invite links  
- Links in restricted channels  

---

# 15. 📊 Technical Details

- Python 3.12  
- discord.py 2.3.2  
- JSON storage  
- Link detection: <100ms  
- Status refresh: 30 seconds  
- Temporary trust check: every minute  

---

# 16. 💡 Best Practices

- Enable logging for mod visibility  
- Add trusted moderators  
- Use temporary trust for events  
- Create a #media or #links channel  
- Use punishment system only when needed  

---

# 17. ⚡ Performance

- Lightweight and optimized  
- Stable across multiple servers  
- Efficient pattern matching  
- Persistent data system  

---

For commands →  
➡️ [Commands Documentation](commands.md)

For setup →  
➡️ [Setup Guide](setup.md)