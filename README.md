<div align="center">

# ☁️ CloudStaff

### Moderation and staff tools for Paper Minecraft servers

**Punishments · Staff utilities · Player records · bStats metrics**

[📖 Wiki & setup guide](https://github.com/LovelyBeeHive/cloudstaff/wiki)

</div>

---

CloudStaff gives your staff team the tools to moderate players and keep useful records, all in one lightweight plugin. Punishments and command history are stored locally so they persist after server restarts.

## ✨ Features

| Category | What you can do |
| --- | --- |
| **Punishments** | Ban, tempban, unban, mute, tempmute, unmute, kick, and warn |
| **Staff tools** | Staff chat, vanish, and freeze or unfreeze players |
| **Player records** | View punishment history and search command history |
| **Configuration** | Customize messages, timezone, appeal text, logging, and freeze settings |
| **Metrics** | Anonymous plugin usage statistics through bStats, with an opt-out setting |

## ⌨️ Commands

| Command | Permission |
| --- | --- |
| `/ban <player> [reason]`, `/tempban <player> <duration> [reason]`, `/unban <player>` | `cloudstaff.ban` |
| `/mute <player> [reason]`, `/tempmute <player> <duration> [reason]`, `/unmute <player>` | `cloudstaff.mute` |
| `/kick <player> [reason]` | `cloudstaff.kick` |
| `/warn <player> <reason>` | `cloudstaff.warn` |
| `/history <player>` | `cloudstaff.history` |
| `/cmdhistory <player> [word] [page]` | `cloudstaff.cmdhistory` |
| `/staffchat [message]` (`/sc`) | `cloudstaff.staffchat` |
| `/vanish` (`/v`) | `cloudstaff.vanish` |
| `/freeze <player>` | `cloudstaff.freeze` |
| `/cloudstaff reload` | `cloudstaff.admin` |

Staff permissions default to operators. You can grant them individually with a permissions plugin such as LuckPerms. Other permission nodes include `cloudstaff.notify`, `cloudstaff.vanish.see`, `cloudstaff.exempt`, and `cloudstaff.nolog`.

## 🚀 Install

1. Use **Paper 26.3+** with **Java 25**.
2. Place `CloudStaff.jar` in your server's `plugins/` folder.
3. Start or restart the server.
4. Customize `plugins/CloudStaff/config.yml` as needed. Run `/cloudstaff reload` after changing it.

Keep `plugins/CloudStaff/cloudstaff.db` when updating the plugin; it holds saved punishments and command history. Back it up before upgrades or manual edits.

## 🔒 Privacy note

Command history can include command arguments. Add your server's private-message and authentication commands to `commands.ignore`, or give sensitive users `cloudstaff.nolog`. Only staff with `cloudstaff.cmdhistory` can search command history.

bStats collection can be disabled by the server owner in `plugins/bStats/config.yml`.

## 📚 Documentation

See the [CloudStaff Wiki](https://github.com/LovelyBeeHive/cloudstaff/wiki) for setup details, configuration, and command and permission reference.
