# 📝 RG AutoMod — Commands

RG AutoMod uses **modern slash commands (/)** and supports **mention-based commands**.

---

## ⚙️ General Commands

### `/help`

Shows all available commands and usage.

---

### `/status`

Displays current server configuration and protection status.

---

## 📋 Whitelist Commands

### `/whitelist add`

Add a domain or pattern to the whitelist.

**Example:**

```
/whitelist add domain:example.com
```

---

### `/whitelist remove`

Remove a domain or pattern from the whitelist.

---

### `/whitelist list`

View all whitelisted domains.

---

## 👤 Trusted System Commands

### `/trust add`

Add a trusted user or role.

**Examples:**

```
/trust add user:@user
/trust add role:@role
```

---

### `/trust remove`

Remove trusted user or role.

---

### `/trust list`

View all trusted users and roles.

---

## 📺 Channel Control Commands

### `/channel allow`

Allow links in a specific channel.

```
/channel allow #media
```

---

### `/channel block`

Remove a channel from the allowlist.

---

### `/channel list`

View allowed channels.

---

## ⚖️ Moderation Commands

### `/strikes view`

View a user's strike count.

---

### `/strikes reset`

Reset a user’s strikes.

---

### `/config punishment`

Configure strike limits and punishment system.

---

### `/config cooldown`

Adjust moderation cooldown settings.

---

### `/config logging`

Set or update log channel.

---

## 🔐 License Commands

### `/license generate`

Generate a license key.

**Example:**

```
/license generate tier:pro duration:3m
```

---

### `/license redeem`

Activate a license key for a server.

---

### `/license status`

Check current license status.

---

## 📊 Utility Commands

### `/stats`

View server moderation statistics.

---

### `/support`

Get support links and resources.

---

## ⚡ Notes

* All commands use `/` (slash commands)
* Mention commands (`@Bot`) are also supported
* Prefix commands like `!` or `.` are **not supported**

---

## 🆘 Need Help?

Join our support server:

👉 https://discord.gg/GFGCn2mMrE

---

Powered by **RG Studios**
