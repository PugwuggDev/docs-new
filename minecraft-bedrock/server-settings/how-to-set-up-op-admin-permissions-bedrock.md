# How to Set Up OP/Admin Permissions (Bedrock)

Giving players operator (OP) or admin permissions on your Bedrock server allows them to use commands like `/gamemode`, `/tp`, or manage other players. This guide shows how to safely grant OP access using the Bedrock permissions system. ✔️

***

### ⛏️ Step 1: Understand Bedrock Permission Levels

Bedrock Edition uses a built-in permission system with four levels:

* **visitor** – Cannot break/place blocks
* **member** – Standard player access
* **operator** – Can use commands and manage players
* **custom** – Advanced permission settings (rarely used)

***

### ➕ Step 2: Add an Operator via Console

* ➡️ Go to your game panel and open the **Console**
* ➡️ Use the command: `op PlayerName`
* ✔️ Replace `PlayerName` with the exact Bedrock username

✅ The player will now have operator permissions next time they join.

***

### ⏰ Step 3: Remove OP Status

To revoke admin access:

* ➡️ Use the command: `deop PlayerName`
* ✔️ This will return the player to standard `member` access

***

### ⚔️ Alternative: Edit permissions.json Manually

You can also assign permissions by editing the `permissions.json` file:

* ➡️ Go to the **File Manager**
* ➡️ Open or create `permissions.json` in the root server directory
* ➡️ Use the format:

```
[
  {
    "permission": "operator",
    "xuid": "1234567890123456"
  }
]
```

✔️ You will need the player’s XUID to use this method.

***

➡️ For help with installation, see our guides on installing addons and plugins. ✅

Need assistance? Reach out to support or open a ticket — we’re here to help. ✔️
