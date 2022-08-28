# InfiniteProjects
Modification of Halo Infinite files to enable hidden game modes.

## IMPORTANT
After you are done with Fiddler, make sure to run "netsh winhttp reset proxy" in administrator CMD!

## Installation
- Step 1: Download Fiddler Classic [https://www.telerik.com/fiddler/fiddler-classic]
- Step 2: Delete everything in your /disk_cache/webcache/ directory in your install folder.
- Step 3: Open an administrator command prompt and run "netsh winhttp set proxy 127.0.0.1:8888]
- Step 4: Run Fiddler.
- Step 5: In Fiddler, go to tools < options, go to HTTPS, and enable "Decrypt HTTPS Traffic".
- Step 6: Back in the main Fiddler window, go to the AutoResponder tab, and enable "Enable rules", "Accept all CONNECTs" and "Unmatched requests passthrough".
- Step 7: Click on Add rule, and make a rule for "/hi/projects/. Respond with the XBOND file you downloaded on the repo.
![image](https://user-images.githubusercontent.com/74399067/187094151-08cbdf23-7f6f-43b7-8d78-79e4f5e126de.png)
- Step 8: Run Halo Infinite and navigate to the custom games menu. You should now see the modes in the "343 Industries" menu.

## FAQ

#### Q: Why doesn't anything microsoft related work? [Game Bar, Microsoft Store]
- A: To fix this, go to WinConfig on the top left in Fiddler, press "Exempt All" and save.

#### Q: I can see the gamemodes, but when I press some they don't show up in the customs menu. Why?
- A: 343 often removes older gamemodes and maps, so if this issue is happening to you, use a newer projects file.

#### Q: How do you create a projects file?
- A: I decompile the gamemode/map manifest included with every Halo Infinite build, and edit them to turn them into a projects file using Infinite Variant Tool.

## Credits
- Soupstream: Creating Infinite Variant Tool [https://github.com/soupstream/InfiniteVariantTool]
- XE_Creature: Showing me how to create projects files.
