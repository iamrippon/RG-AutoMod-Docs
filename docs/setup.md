# ⚙️ RG AutoMod — Setup Guide

RG AutoMod is designed to work instantly with zero configuration.  
However, server administrators can customize the bot using the commands listed below.

---

# 1. 🚀 Invite the Bot

Use the official invite link:

https://discord.com/oauth2/authorize?client_id=1447209989683806400&permissions=388160&scope=bot%20applications.commands

The bot will automatically:
- Load default whitelist
- Begin blocking unwanted links
- Send a welcome message with setup info

---

# 2. 📊 Enable Logging (Optional but Recommended)

Logging helps moderators see which links were blocked.

/set-log-channel #logs

bash
Copy code

To disable:
/remove-log-channel

yaml
Copy code

---

# 3. 👤 Add Trusted Users

Allow users to post links anywhere in the server.

### Permanent trust:
/trust-user @user

shell
Copy code

### Temporary trust:
/trust-user @user 1h

yaml
Copy code

Remove trust:
/untrust-user @user

bash
Copy code

View trusted users:
/list-trusted

yaml
Copy code

---

# 4. 📺 Configure Allowed Channels

Allow all links in specific channels only.

Allow a channel:
/allow-channel #channel

css
Copy code

Block a channel:
/block-channel #channel

yaml
Copy code

List allowed channels:
/list-channels

yaml
Copy code

---

# 5. 🔗 Add Custom Whitelisted Links

Add your own allowed links/domains.

/add-whitelist discord.gg
/add-whitelist twitter.com
/add-whitelist example.com/promo

makefile
Copy code

Remove:
/remove-whitelist pattern

makefile
Copy code

List:
/list-whitelist

css
Copy code

Reset to defaults:
/reset-whitelist

yaml
Copy code

---

# 6. ⚖️ Enable Auto-Punishment (Optional)

Automatically punish users who repeatedly post blocked links.

Enable:
/punishment enable

makefile
Copy code

Disable:
/punishment disable

makefile
Copy code

Configure:
/punishment-config 3 10

sql
Copy code
(3 strikes → 10-minute timeout)

Reset user strikes:
/reset-strikes @user

yaml
Copy code

---

# 7. 💬 Customize Warning Messages

Default warning works fine, but you can customize it.

Set custom message:
/set-warning Your message here!

vbnet
Copy code

Reset to default:
/reset-warning

yaml
Copy code

---

# 8. 📈 View Server & Bot Statistics

Use `/status` to view:

- Total servers  
- Total users  
- Bot ping  
- Trusted users  
- Allowed channels  
- Whitelist patterns  
- Logging enabled/disabled  
- Punishment configuration  

Example:
/status

yaml
Copy code

---

# 9. 🛠 Bot Behavior Overview

RG AutoMod will allow links if:
- User is trusted  
- Channel is allowed  
- Link matches whitelist  
- User is an admin  

Otherwise → the link is deleted.

---

# ✔ Your Bot is Ready!

Most servers only need:
- `/set-log-channel #logs`  
- `/allow-channel #links`  
- `/trust-user @mods`  

The rest is optional.

---

For full feature descriptions →  
➡️ [Features Documentation](features.md)

For command list →  
➡️ [Commands Guide](commands.md)