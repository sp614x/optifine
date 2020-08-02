---
name: Bug report
about: Help OptiFine pinpoint issues
title: "[Category] Short description"
labels: ''
assignees: ''

---

## Description of Issue
Please provide as much detail as possible.

## Steps to Reproduce
1. What do you do... 
2. ...to find this bug?

## OptiFine Version
Self-explanatory. 

## Installation Method
How did you install OptiFine? Did you use the included standalone installer, or did you drop the JAR file into your "mods" folder?

## Fabric/Forge Version
**If OptiFine is installed as standalone, you can remove this section.**

## OptiFabric Version
**If OptiFine is installed as standalone, or you're using Forge, you can remove this section.**

## Other Installed Mods
*Every* single mod you have installed, besides OptiFine. Please don't leave anything out, even if you think it has nothing to do with the issue at hand. For long lists of mods, use Pastebin. https://pastebin.com/

**If OptiFine is installed as standalone, remove this section.**

## Log Files/Crash Reports
Any relevant log files. Drag and drop text files here to upload to GitHub directly, OR upload the complete contents to Pastebin. https://pastebin.com/

You can get logs from `.minecraft/logs`, and crash reports from `.minecraft/crash-reports`. 
Locating your `.minecraft` folder will depend entirely on your OS. See this page for details: https://minecraft.gamepedia.com/.minecraft

**DO NOT directly copy and paste log contents here on GitHub.**

## F3 Debug Screenshot
Minecraft's built-in debug screen provides *a lot* of useful information, and should be included even if the issue is not something that can be captured in a still image.

To open this menu, simply press `F3` on your keyboard while in-game. Please ensure the text is easily readable. Depending on the size/resolution of your monitor, you may have to adjust your GUI scale for all text to be completely visible on-screen.

## Prior Testing
If you've installed standalone:
- Does this happen in Vanilla without OptiFine?

If you've installed using Forge/Fabric:
- Does this happen without other mods installed? 
   - Only OptiFine and Forge
   - Only OptiFine, OptiFabric, and Fabric
- Does this happen without any mods at all?
   - Only Forge/Fabric by itself.
- Does this happen in OptiFine standalone?
- Does this happen in Vanilla without OptiFine?
- Have you tried using a binary search to find which mods cause this issue?
   - To find conflicting mods, split your mods into 2 groups (not including OptiFine/OptiFabric, obviously). Remove one group, and test in-game. Keep the group that has the problem, and repeat until no more mods can be removed without the issue disappearing.
   - Does the issue still happen with only the remaining mods installed?
      - Forge/Fabric and remaining mods, without OptiFine

## Additional Information
Here goes any final remarks and everything else that might not fit in the previous sections.
