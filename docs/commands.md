# 📝 RG AutoMod — Commands Documentation

This page lists all available slash commands for RG AutoMod, organized by category for server administrators and moderators.

---

# 1. 👤 User Trust Commands

### Grant link posting permission:
/trust-user @user

shell
Copy code

### Grant temporary link permission:
/trust-user @user [duration]

sql
Copy code
Examples:
- /trust-user @John 30m
- /trust-user @Winner 1h
- /trust-user @Guest 2d

### Remove trust:
/untrust-user @user

shell
Copy code

### View all trusted users:
/list-trusted

yaml
Copy code
Shows:
- Permanent trusted users  
- Temporary trusted users (with expiry timers)

---

# 2. 📺 Channel Allowlist Commands

### Allow links in a channel:
/allow-channel #channel

shell
Copy code

### Block links in a channel:
/block-channel #channel

shell
Copy code

### List all allowed channels:
/list-channels

yaml
Copy code

---

# 3. 🔗 Whitelist Management Commands

### Add a custom allowed link/domain:
/add-whitelist pattern

shell
Copy code

### Remove a custom allowed pattern:
/remove-whitelist pattern

shell
Copy code

### View all whitelist patterns:
/list-whitelist

shell
Copy code

### Reset to default whitelist only:
/reset-whitelist

yaml
Copy code

---

# 4. 📊 Logging Commands

### Enable link deletion logging:
/set-log-channel #channel

shell
Copy code

### Disable logging:
/remove-log-channel

yaml
Copy code

---

# 5. 💬 Warning Message Commands

### Set a custom warning message:
/set-warning message

shell
Copy code

### Reset warning message to default:
/reset-warning

yaml
Copy code

---

# 6. ⚖️ Auto-Punishment Commands (Optional Feature)

### Enable or disable the punishment system:
/punishment enable
/punishment disable

shell
Copy code

### Configure strike limit and timeout duration:
/punishment-config [max_strikes] [timeout_minutes]

shell
Copy code

### Reset a user's strike count:
/reset-strikes @user

yaml
Copy code

---

# 7. 📈 Status & Information Commands

### View bot statistics and server configuration:
/status

shell
Copy code

### Show help info and command guide:
/help

yaml
Copy code

---

# ✔ Command Syntax Notes
- All commands require **Administrator** permissions to modify settings  
- Duration formats: `15s`, `30m`, `1h`, `2d`  
- Pattern matching for whitelists is case-insensitive  

---

For full detailed descriptions of features →  
➡️ [Full Feature Documentation](features.md)

For setup instructions →  
➡️ [Setup Guide](setup.md)