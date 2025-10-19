# How to Enable/Disable Whitelist (Bedrock)

Enabling the whitelist ensures that only approved players can join your Bedrock server. This is especially useful for private communities, staff-only setups, or family servers. ✔️

***

### ⛏️ What Is a Whitelist?

The whitelist is a list of allowed player usernames. When enabled, only players on that list can join your server. Everyone else will receive a message saying they are not whitelisted. ⚠️

***

### ➕ How to Enable the Whitelist

* ➡️ Log into your control panel
* ➡️ Go to the **File Manager**
* ➡️ Open `server.properties`
* ➡️ Find the line `white-list=false` and change it to `true`
* ✔️ Save and restart the server to apply the change

✅ The whitelist is now enabled — only players you add to it can join.

***

### ⚔️ How to Add or Remove Players

* ➡️ Open the **Console** in your game panel
* ➡️ Use the command: `whitelist add PlayerName`
* ✔️ Repeat this for each player you want to allow
* ➡️ To remove someone, use: `whitelist remove PlayerName`

***

### ➖ How to Disable the Whitelist

* ➡️ Return to `server.properties`
* ➡️ Change `white-list=true` back to `false`
* ➡️ Save and restart the server

✔️ Disabling the whitelist allows any player to join (based on other access settings).

***

➡️ For help with installation, see our guides on installing addons and plugins. ✅

Need assistance? Feel free to reach out or open a support ticket — we’re happy to help. ✔️
