# 📜 RG AutoMod — Changelog

This document tracks all updates, improvements, and major changes made to the bot.

---

# 🟦 v3.0.0 — Database & System Upgrade (Major Update)

### 🚀 Core Upgrades

* Migrated from JSON storage → **SQLite database (bot.db)**
* Introduced modular database system (`database.py`)
* Improved data reliability and persistence
* Removed dependency on JSON-based storage

---

### ⚡ Performance Improvements

* Optimized moderation workflow
* Reduced redundant operations
* Improved response time under load
* Better handling of active servers

---

### 🧠 System Improvements

* Improved configuration handling
* Enhanced whitelist and channel control system
* Better trusted user & role management
* More stable cooldown and moderation logic

---

### 📊 Logging & Monitoring

* Improved logging system
* More consistent moderation logs
* Better tracking of user violations

---

### 🔄 Bot Improvements

* Updated command system (slash + mention support)
* Cleaner command handling and reduced console spam
* Improved bot stability and error handling
* Dynamic rotating status with live stats

---

### 💾 Storage System

* Fully database-driven storage system
* Persistent storage for:

  * whitelist
  * trusted users & roles
  * allowed channels
  * configuration settings
  * user violations

---

### 🧪 Fixes & Stability

* Fixed multiple runtime errors
* Reduced crash scenarios
* Improved overall reliability

---

# 🟩 v2.x.x — Internal Improvements

*(Internal builds and testing phase)*

* Initial database experiments
* System restructuring
* Early performance optimizations

---

# 🟦 v1.0.0 — Public Release (Initial Launch)

### 🚀 Core Features

* Complete automatic link detection system
* Real-time link deletion with customizable warnings
* Default whitelist (essential safe domains only)
* Custom whitelist support
* Channel allowlist system
* Permanent & temporary trusted user system
* Link deletion logging system
* Welcome message on server join
* Dynamic status rotation

---

### ⚖️ Moderation Features

* Optional auto-punishment system

  * Strike-based
  * Timeout enforcement
  * Automatic strike reset
* Strike tracking system

---

### 🛠 Configuration Commands

* Set/remove log channel
* Custom warning system
* Whitelist management
* Channel control system
* Trusted users system
* `/status` dashboard

---

### 💾 Storage System

* JSON-based data storage (legacy system)
* Automatic data saving and loading

---

### 📚 Documentation

* Initial GitHub documentation
* Setup, commands, and feature guides

---

# 🟪 Upcoming Roadmap

Planned future improvements:

* Advanced analytics dashboard
* Improved UI/UX for commands
* Performance optimizations (caching system)
* Expanded moderation controls
* Dashboard / web panel (long-term)

---

## 🆘 Feedback & Requests

Have ideas or feature requests?

👉 https://discord.gg/GFGCn2mMrE

---

Powered by **RG Studios**
