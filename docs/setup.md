# ⚙️ RG AutoMod — Setup Guide

This guide will help you set up **RG AutoMod** in your Discord server in just a few steps.

---

## 🚀 Step 1 — Invite the Bot

Invite RG AutoMod to your server using the official link.

Once invited:

* The bot will join your server
* A welcome message will be sent with basic instructions

---

## 🛠 Step 2 — Required Permissions

Make sure the bot has the following permissions:

* Manage Messages
* Moderate Members (for timeouts)
* View Channels
* Send Messages
* Embed Links
* Read Message History

👉 Without these, the bot may not function properly.

---

## 📋 Step 3 — Basic Setup

### 1️⃣ Set Log Channel

```bash
/set-log-channel #logs
```

This is required to track moderation actions.

---

### 2️⃣ Allow Channels (Optional)

Allow links in specific channels:

```bash
/allow-channel #media
```

---

### 3️⃣ Add Trusted Users / Roles

Allow trusted users to bypass protection:

```bash
/trust add user:@user
/trust add role:@role
```

---

### 4️⃣ Add Custom Whitelist

Allow safe links:

```bash
/whitelist add domain:example.com
```

---

## ⚖️ Step 4 — Configure Moderation

Set punishment system:

```bash
/config punishment
```

You can configure:

* Strike limits
* Timeouts
* Reset behavior

---

## 🔄 Step 5 — Verify Setup

Use:

```bash
/status
```

Check:

* Log channel ✔
* Protection enabled ✔
* Whitelist ✔
* Trusted system ✔

---

## ⚡ Quick Setup (Recommended)

If available, use:

```bash
/setup quick
```

👉 Automatically configures:

* Log channel
* Basic protection
* Default settings

---

## ❗ Common Mistakes

### Bot not deleting links

* Check permissions
* Ensure bot role is above users

---

### Logs not showing

* Re-set log channel
* Check channel permissions

---

### Commands not working

* Use slash commands `/`
* Ensure bot is online

---

## 🧠 Tips

* Keep bot role **above regular members**
* Use whitelist for safe domains
* Avoid over-restricting channels

---

## 🆘 Need Help?

Join support:

👉 https://discord.gg/GFGCn2mMrE

---

Powered by **RG Studios**
