<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>RG AutoMod – Discord Moderation Bot</title>
<style>
    body {
        font-family: "Segoe UI", sans-serif;
        background: #0f0f10;
        color: #e5e5e5;
        margin: 0;
        padding: 0;
        line-height: 1.6;
    }

    .container {
        max-width: 900px;
        margin: auto;
        padding: 40px 20px;
    }

    h1, h2, h3 {
        color: #ffffff;
        margin-bottom: 10px;
    }

    h1 {
        font-size: 40px;
        text-align: center;
        margin-bottom: 30px;
        font-weight: 700;
    }

    .section {
        background: #1a1a1d;
        padding: 25px;
        border-radius: 10px;
        margin-bottom: 25px;
        border: 1px solid #2c2c30;
    }

    .badge {
        display: inline-block;
        padding: 6px 14px;
        border-radius: 20px;
        font-size: 13px;
        margin-right: 6px;
        margin-bottom: 10px;
        background: #29292e;
        border: 1px solid #3a3a40;
    }

    a {
        color: #4ba3ff;
        text-decoration: none;
        font-weight: 500;
    }

    a:hover {
        text-decoration: underline;
    }

    .code-box {
        background: #111113;
        padding: 12px;
        border-radius: 6px;
        border: 1px solid #2c2c30;
        overflow-x: auto;
        margin: 10px 0;
        font-family: monospace;
        white-space: pre;
        color: #d1d1d1;
    }
</style>
</head>

<body>

<div class="container">

<h1>🤖 RG AutoMod – Discord Link Moderation Bot</h1>

<div class="section">
    <span class="badge">Bot Status: Live</span>
    <span class="badge">Docs Completed</span>
    <span class="badge">Closed Source</span>
    <span class="badge">Secure</span>
</div>

<div class="section">
    <h2>📌 Overview</h2>
    <p>
        RG AutoMod is a clean, fast, and powerful Discord bot designed to block unwanted links, spam, and scam URLs.
        It provides an automated link-protection system with trusted users, channel allowlists, custom whitelists, and optional strike-based punishment.
        Everything is fully slash-command based and requires zero setup.
    </p>
</div>

<div class="section">
    <h2>🚀 Invite the Bot</h2>
    <p>Use the official invite link:</p>

    <div class="code-box">
https://invite-rgautomod.rixstongamer.xyz
    </div>
</div>

<div class="section">
    <h2>✨ Main Features</h2>

    <h3>1. Automatic Link Blocking</h3>
    <ul>
        <li>Detects all major URL formats</li>
        <li>Instant message deletion</li>
        <li>Temporary warning message (auto-deletes)</li>
    </ul>

    <h3>2. Default Safe Whitelist</h3>
    <p>Some safe links are always allowed (e.g., official website, YouTube, Instagram).</p>

    <h3>3. Trusted User System</h3>
    <ul>
        <li>Permanent trust</li>
        <li>Temporary trust (15s, 30m, 1h, 2d, etc.)</li>
        <li>View and remove trusted users</li>
    </ul>

    <h3>4. Channel Allowlist</h3>
    <p>Allow links only in selected channels (/allow-channel).</p>

    <h3>5. Custom Whitelist Rules</h3>
    <p>Add or remove custom domains or link patterns.</p>

    <h3>6. Logging System</h3>
    <p>Track link deletion with full details (user, channel, message, timestamp, strikes).</p>

    <h3>7. Auto-Punishment System</h3>
    <p>Configurable strike-based timeout system (optional).</p>

    <h3>8. Persistent Storage</h3>
    <p>All settings are saved and restored even after restarts.</p>

    <h3>9. Dynamic Status</h3>
    <p>Status updates every 30 seconds with server count.</p>

    <h3>10. Automatic Welcome Message</h3>
    <p>Provides basic setup instructions when joining a new server.</p>
</div>

<div class="section">
    <h2>🧩 Commands Overview</h2>

    <h3>User Trust</h3>
    <div class="code-box">
/trust-user @user  
/trust-user @user 1h  
/untrust-user @user  
/list-trusted
    </div>

    <h3>Channel Allowlist</h3>
    <div class="code-box">
/allow-channel #channel  
/block-channel #channel  
/list-channels
    </div>

    <h3>Whitelist Management</h3>
    <div class="code-box">
/add-whitelist pattern  
/remove-whitelist pattern  
/list-whitelist  
/reset-whitelist
    </div>

    <h3>Logging</h3>
    <div class="code-box">
/set-log-channel #channel  
/remove-log-channel
    </div>

    <h3>Warnings</h3>
    <div class="code-box">
/set-warning message  
/reset-warning
    </div>

    <h3>Punishment</h3>
    <div class="code-box">
/punishment enable  
/punishment disable  
/punishment-config strikes timeout  
/reset-strikes @user
    </div>
</div>

<div class="section">
    <h2>📄 Documentation</h2>
    <ul>
        <li><a href="docs/overview.md">Overview</a></li>
        <li><a href="docs/features.md">Features</a></li>
        <li><a href="docs/commands.md">Commands</a></li>
        <li><a href="docs/setup.md">Setup Guide</a></li>
        <li><a href="docs/permissions.md">Permissions</a></li>
        <li><a href="docs/changelog.md">Changelog</a></li>
        <li><a href="docs/support.md">Support</a></li>
    </ul>
</div>

<div class="section">
    <h2>🔐 License</h2>
    <p>
        RG AutoMod is a closed-source proprietary bot.
        Redistribution of code is not allowed. Documentation is public for reference.
    </p>
</div>

<div class="section">
    <h2>🆘 Support</h2>
    <p>Official support server:</p>
    <div class="code-box">
https://dsc.gg/rixstongamer
    </div>
</div>

</div>

</body>
</html>
