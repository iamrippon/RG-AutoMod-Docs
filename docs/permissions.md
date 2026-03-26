# 🔐 RG AutoMod — Permissions Guide

This document explains all permissions required by **RG AutoMod** and why they are needed.

---

## ⚙️ Required Permissions

RG AutoMod needs the following permissions to function correctly:

### 📝 Manage Messages

* Delete harmful links and spam
* Enforce link moderation

---

### ⏱️ Moderate Members

* Apply timeouts for rule violations
* Enforce punishment system

---

### 👀 View Channels

* Read messages across the server
* Monitor activity

---

### 💬 Send Messages

* Send warnings and system messages
* Respond to commands

---

### 🔗 Embed Links

* Send rich embeds (logs, status, alerts)

---

### 📜 Read Message History

* Analyze recent messages for moderation
* Ensure accurate detection

---

## ⚠️ Recommended Permissions

These are not strictly required but improve functionality:

### 🛠️ Manage Roles

* Assign or manage roles (future features)
* Required for advanced moderation systems

---

### 📢 Manage Channels (Optional)

* Used for advanced features like raid protection (if enabled)

---

## 🚫 Permissions Not Used

RG AutoMod does **NOT** require or use:

* Administrator
* Manage Server
* Kick Members (unless future features require it)

👉 The bot is designed to use **only necessary permissions** for security and trust.

---

## ⚠️ Role Position (IMPORTANT)

For RG AutoMod to work correctly:

* The bot’s role must be **above regular members**
* The bot’s role must be **above users it needs to moderate**

Otherwise:

* It may fail to delete messages
* It may fail to apply punishments

---

## 🧠 Best Practices

* Do NOT give Administrator permission
* Only grant required permissions
* Regularly review bot permissions

---

## 🆘 Troubleshooting

### Bot not deleting links

* Check "Manage Messages" permission
* Ensure role hierarchy is correct

---

### Punishments not working

* Check "Moderate Members" permission
* Ensure bot role is high enough

---

### Logs not appearing

* Check channel permissions
* Ensure bot can send messages

---

## 🆘 Need Help?

Join support:

👉 https://discord.gg/GFGCn2mMrE

---

Powered by **RG Studios**
