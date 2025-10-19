# Installing Forge or Fabric on Your Minecraft Server

Mod loaders like Forge and Fabric are essential for running mods on your Minecraft server. This guide shows you how to install and configure these mod loaders using HostByte's Game Panel. ⛏️

***

### ⚙️ What are Mod Loaders?

Mod loaders are frameworks that allow mods to run on Minecraft:

* ✔️ **Forge** - Most popular, supports most mods
* ✔️ **Fabric** - Lightweight, faster updates
* ✔️ **NeoForge** - Forge fork for newer versions
* ✔️ **Quilt** - Fabric alternative

***

### ⚙️ Forge vs Fabric Comparison

Understanding the differences between mod loaders:

| **Feature**        | **Forge**             | **Fabric**              |
| ------------------ | --------------------- | ----------------------- |
| **Mod Support**    | Extensive (most mods) | Growing (many new mods) |
| **Performance**    | Good                  | Excellent               |
| **Update Speed**   | Slower                | Faster                  |
| **Stability**      | Very stable           | Stable                  |
| **Learning Curve** | Moderate              | Easier                  |

***

### ⚠️ Important: Version Compatibility

Always ensure compatibility between:

* ⚠️ **Minecraft Version** - Your server version
* ⚠️ **Mod Loader Version** - Forge/Fabric version
* ⚠️ **Mod Versions** - All mods must be compatible
* ⚠️ **Server Software** - Paper/Spigot compatibility

**⭐ Tip:** Most modpacks come with pre-configured versions, but custom setups require careful version matching.

***

### ⚙️ Method 1: Installing Forge

Step-by-step Forge installation:

#### ⚙️ Step 1: Download Forge

1. ➡️ Visit [Forge Official Site](https://files.minecraftforge.net/)
2. ➡️ Select your Minecraft version
3. ➡️ Download the "Installer" version
4. ➡️ Choose "Server" installation

#### ⚙️ Step 2: Install on Server

1. ➡️ Upload the Forge installer to your server (see our [File Manager Guide](https://www.hostbyte.net/billing/knowledgebase/75/How-to-Use-the-File-Manager.html))
2. ➡️ Run the installer via console (see our [Console Guide](https://www.hostbyte.net/billing/knowledgebase/74/How-to-Use-the-Console.html))
3. ➡️ Accept the EULA
4. ➡️ Start the server to generate files

#### ⚙️ Step 3: Configure Startup

Update your server startup command in the Game Panel:

`java -Xms2G -Xmx4G -jar forge-1.19.2-43.2.0.jar nogui`

***

### ⚙️ Method 2: Installing Fabric

Step-by-step Fabric installation:

#### ⚙️ Step 1: Download Fabric

1. ➡️ Visit [Fabric Server](https://fabricmc.net/use/server/)
2. ➡️ Select your Minecraft version
3. ➡️ Download the Fabric server JAR
4. ➡️ Download Fabric API (required)

#### ⚙️ Step 2: Install on Server

1. ➡️ Upload Fabric server JAR to your server (see our [File Manager Guide](https://www.hostbyte.net/billing/knowledgebase/75/How-to-Use-the-File-Manager.html))
2. ➡️ Rename it to "fabric-server.jar"
3. ➡️ Upload Fabric API to mods folder
4. ➡️ Start server to generate files

#### ⚙️ Step 3: Configure Startup

Update your server startup command:

`java -Xms2G -Xmx4G -jar fabric-server.jar nogui`

***

### ⚙️ Method 3: Using HostByte's One-Click Installers

HostByte's Game Panel offers easy installation:

1. ➡️ Access your HostByte control panel (see our [Game Panel Access Guide](https://www.hostbyte.net/billing/knowledgebase/73/How-to-Access-Your-Game-Panel.html))
2. ➡️ Go to "Startup" settings
3. ➡️ Select "Forge" or "Fabric" from dropdown
4. ➡️ Choose your Minecraft version
5. ➡️ Click "Save" and restart server

***

### ⚙️ Installing Mods

Once your mod loader is installed:

#### ⚙️ Forge Mods

1. ➡️ Download mod JAR files
2. ➡️ Upload to "mods" folder
3. ➡️ Ensure version compatibility
4. ➡️ Restart server

#### ⚙️ Fabric Mods

1. ➡️ Download Fabric mod JAR files
2. ➡️ Upload to "mods" folder
3. ➡️ Install required dependencies
4. ➡️ Restart server

***

### ⚙️ Essential Configuration

Important settings for modded servers:

#### ⚙️ server.properties

* ✔️ **max-players** - Reduce for modded servers
* ✔️ **view-distance** - Lower for better performance
* ✔️ **simulation-distance** - Balance performance
* ✔️ **spawn-protection** - Protect spawn area

#### ⚙️ JVM Arguments for Mods

Optimized arguments for modded servers:

`-Xms2G -Xmx4G -XX:+UseG1GC -XX:+ParallelRefProcEnabled -XX:MaxGCPauseMillis=200 -XX:+UnlockExperimentalVMOptions -XX:+DisableExplicitGC -XX:+AlwaysPreTouch -XX:G1NewSizePercent=30 -XX:G1MaxNewSizePercent=40 -XX:G1HeapRegionSize=8M -XX:G1ReservePercent=20 -XX:G1HeapWastePercent=5 -XX:G1MixedGCCountTarget=4 -XX:InitiatingHeapOccupancyPercent=15 -XX:G1MixedGCLiveThresholdPercent=90 -XX:G1RSetUpdatingPauseTimePercent=5 -XX:SurvivorRatio=32 -XX:+PerfDisableSharedMem -XX:MaxTenuringThreshold=1`

***

### ⚠️ Common Installation Issues

Solutions for frequent problems:

* ⚠️ **Server Won't Start** - Check JAR file name and startup command
* ⚠️ **Mods Not Loading** - Verify mod versions match loader
* ⚠️ **Out of Memory** - Increase RAM allocation
* ⚠️ **Version Conflicts** - Ensure all components match
* ⚠️ **Missing Dependencies** - Install required libraries

***

### ⚙️ Performance Tips

Optimize your modded server performance:

* ✔️ **Allocate Adequate RAM** - Mods need more memory
* ✔️ **Use Optimized JVM Arguments** - Better garbage collection
* ✔️ **Limit Mod Count** - More mods = more resources
* ✔️ **Regular Restarts** - Clear memory leaks
* ✔️ **Monitor Resource Usage** - Watch RAM and CPU

***

### ✅ Getting Help

If you need assistance with your control panel:

* ✅ **Knowledge Base** - Check our comprehensive guides
* ✅ **Support Ticket** - Submit a ticket for technical issues
* ✅ **Discord** - [HostByte Discord](https://discord.gg/9q8xRVnqXh)
* ✅ **Community Forum** - Connect with other server owners
* ✅ **Video Tutorials** - Coming soon

***

### ✅ Ready to Install Your Mod Loader?

Now that you understand how to install Forge and Fabric, you're ready to start adding mods to your server! Choose the right mod loader for your needs, follow the installation steps, and begin creating your custom Minecraft experience. ✅
