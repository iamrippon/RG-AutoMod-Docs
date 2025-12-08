# 🔐 RG AutoMod — Permission Requirements

RG AutoMod is designed to run safely with minimal permissions.  
This page explains each required permission and why it is needed.

---

# 1. ✔ Required Permissions (Must Be Enabled)

### **Manage Messages**
- Allows the bot to delete messages containing blocked links  
- Required for the entire moderation system to function  

### **Send Messages**
- Allows the bot to send warnings, logs, and status updates

### **Embed Links**
- Required for sending rich embeds in logs, welcome messages, and help messages

### **Read Message History**
- Allows the bot to properly reference and delete messages  
- Required for accurate link detection

### **View Channels**
- Needed so the bot can see channels and apply rules

### **Use Application Commands**
- Allows slash commands (`/help`, `/trust-user`, `/allow-channel`, etc.)

---

# 2. ✔ Optional (Recommended) Permissions

### **Attach Files**
- Used for detailed logging or future features

### **Use External Emojis**
- Allows better-looking embeds and warning messages  

---

# 3. ❌ Permissions NOT Required (Do NOT Give)

RG AutoMod does **NOT** need any of the following:

- Administrator  
- Manage Server  
- Manage Roles  
- Manage Channels  
- Ban Members  
- Kick Members  
- Moderate Members  
- Mention Everyone  
- Manage Webhooks  
- View Audit Log  

Giving unnecessary permissions may cause:
- Security issues  
- User concern  
- Top.gg review delays  

---

# 4. ⚠️ Timeout Permission (If Punishment System Is Enabled)

If you want to use the optional auto-punishment system:

### Required:
**Moderate Members** (Timeout Members)

Used ONLY to issue timeouts after repeated link violations.

If punishment system is disabled → this permission is not needed.

---

# 5. ✔ Final Permissions Summary

| Permission | Required | Reason |
|-----------|----------|--------|
| Manage Messages | ✔ | Delete blocked links |
| Send Messages | ✔ | Warnings + messages |
| Embed Links | ✔ | Status, logs, help embeds |
| Read Message History | ✔ | Detect and delete messages |
| View Channels | ✔ | See channels and enforce rules |
| Use Application Commands | ✔ | Slash commands |
| Attach Files | Optional | Better logging |
| Use External Emojis | Optional | Aesthetic embeds |
| Moderate Members | Optional | Timeout system |

---

# 6. 💡 Recommended Invite Permissions

Use this safe pre-calculated permission integer:

388160

yaml
Copy code

This ensures:
- No dangerous permissions  
- Top.gg friendly  
- Maximum security  

Official invite link:
https://discord.com/oauth2/authorize?client_id=1447209989683806400&permissions=388160&scope=bot%20applications.commands

---

For setup →  
➡️ [Setup Guide](setup.md)

For full features →  
➡️ [Feature Documentation](features.md)