# How to Set Up OP/Admin Permissions

Giving a player OP (operator) status allows them to run administrative commands like `/gamemode`, `/tp`, and `/ban`. You can assign OP using the console or by editing a file directly. ✔️

***

### ⛏️ Option 1: Using the Console

* ➡️ Go to your server's **Console** tab
* ➡️ Type the following command and press Enter:

```
op PlayerName
```

✔️ Replace `PlayerName` with the exact username of the player.

***

### ⛏️ Option 2: Using the `ops.json` File

If your server is offline, or you prefer to add OP manually:

* ➡️ Go to **File Manager**
* ➡️ Open the file called `ops.json` (in the root folder)
* ➡️ Add your player’s entry in this format:

```
[
  {
    "uuid": "player-uuid-here",
    "name": "PlayerName",
    "level": 4,
    "bypassesPlayerLimit": false
  }
]
```

✔️ You can get a player’s UUID from [https://mcuuid.net](https://mcuuid.net/).

***

### ⏰ Step 3: Restart the Server

After assigning OP, restart the server for the change to take effect:

* ➡️ Go to the **Console**
* ➡️ Click **Restart**

***

### ❗ What OP Levels Mean

OP level can be set from 1 to 4:

* ✔️ Level 1: Basic commands like `/gamemode` and `/tp`
* ✔️ Level 2: Can use command blocks
* ✔️ Level 3: Can kick or ban players
* ✔️ Level 4: Full admin permissions

➡️ If you use a plugin like LuckPerms, OP is not required — use plugin permissions instead.

***

### ❌ Removing OP

To remove OP from a player:

* ➡️ Use the console command:

```
deop PlayerName
```

✔️ This immediately removes their admin access.

Need help assigning permissions or using plugins instead of OP? Our support team is happy to assist. ✅
