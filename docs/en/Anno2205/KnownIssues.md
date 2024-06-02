# Known Issues

**Base game:**

- The four new products (Organic Food, Fine Food, Sustenance Packs and Thermal Shells) cannot be traded with the world market. 
- There are five quests to guide you to do specific research to unlock certain buildings as the "Unlock Condition" tooltip only works with population milestones. Unfortunately those quests will be visible in all sessions, not only in those the buildings are located in.
- Certain Secondary Module tooltips will not show the correct tooltip description (i.e. Energy module on Energy Production buildings giving +15% output, or Mars Research Lab modules)
- The population overview filter in the strategic view does not work properly with the new Arctic Tier 3. It does not show the correct portrait next to the number. Same goes for the Martian Synthetics.
- Services are a new "product". The balance can not be shown in the "usual" balance menu, otherwise they would be tradeable via trade route. Instead you can find them in the building material bar at the top or click on any Public Building and hover over the "Globe" icon to see the current sector balance.
- Company Headquarter infotip in the bottom of the screen seems to be hardcoded and displays tier 2, 3 and 4 public needs although those have been removed from the game.
- Factories that produce Urbanisation as a site-product cannot be paused anymore.
- Selecting a mining site on the Moon will only show 5 possible entries in the UI. As there are now 6 mines in total, the Regolith Gatherer can only be build via buildmenu.
- Increased storage for Rare Resource Generators only comes into effect after collecting the resources once. Therefore always wait until the first unit has been generated and collect it immediately after building to set the storage amount to the modded one.

**Mars Sector:** Due to the way, Mars Sector is coded to be part of the Moon region, some issues arise from this specifically:

- Mars sector takes longer than other sectors to load.
- The unlock notification for new buildings on the Moon has been changed, so that all newly unlocked Moon buildings will show up as "New Moon Buildings" in the notification.
- To manage the build menu and to restrict Mars buildings to the Mars sector, I had to use a workaround by locking the Moon buildings when entering the Mars session. When you leave the Mars session (for example to adjust trade routes), you will get a notification, that again "New Moon Buildings" have been unlocked. I already shortened the notification by using the "New Moon Buildings" pool, but if I disable them completely, you will get no notification on first unlock.
- After entering the Mars sector and open the build menu, you regularly need to select "Martian Synthetics" tab again to see the available buildings.
- Pressing the Hotkey for "Build Street" on the Mars will result in the Moon Tracks instead of the expected Mars Tracks. Pipette it or use the build menu entry to lay down Mars Tracks instead.
- Using the buildings filter tab next to the minimap (the population button) in the Mars Session will lead to a game freeze, only resolvable by killing the task.
- The Mars sector has some unique sector traits available. Notice, that on entering the sector, the welcome UI shows a random Moon trait instead of the Martian one. That one will only be given to the sector on first enter. You can reroll the sector trait by completing a special quest. This involves delivering certain products to your space port. Notice that the usual way of rerolling sector traits will result in a random trait from the Moon!
- Mars Meteors use Moon ground textures.
- While loading the Mars Sector icon will change to a white rectangle. After clicking for loading, click anywhere on the strategic view again to get the icon back.
- Whenever Mars season changes and you are in another sector, the time of day will change to that one used by the Martian season effect on its own accord. You can adjust the time via the camera menu next to the minimap.
- If you use the Geo-Engineering quest on Mars, the script may randomly choose to apply the same trait that is already active. This will cause the sector to lose its trait altogether. In that case, you can use the console to reapply the effect. The GUIDs can be found [here](/en/Anno2205/SectorTraits.md). First, enter the Mars session. Now press Shift+F1 to open the console and type `debug.toggleSectorEffect(GUID)` using the corresponding number of the wanted trait. Press enter and close the console with Shift+F1 again.
- Sometimes, Martian Season effects can randomly start on the Moon. This is a problem, as they last for a very long time and cannot be resolved with a quest. Again, you need to use the console to get rid of them, if it happens to you: First, enter the Moon session in question. Now press Shift+F1 to open the console and type `debug.toggleSectorEffect(GUID)`. Proceed to replace the "GUID" placeholder with the corresponding GUID from the currently active season effect (see below). Press enter and close the console with Shift+F1 again. The effect should be gone.
- Sometimes, Martian Season effects can end up mismatched with the current season quest. If you currently suffer from mismatched season effect to the shown season quest in the quest tracker on the left side of the screen, you have to use the console to fix this:
> 1. Press Shift+F1 to open the console.
> 2. Enter (without any typing errors, pay attention to upper and lower case!), replace "CurrentSeasonGUID" with the correct number from the table below:
`debug.startSectorEffect(CurrentSeasonGUID,19990093)`
> 3. Press Enter
> 4. Enter (without any typing errors, pay attention to upper and lower case!), , replace "CorrectSeasonGUID" with the correct number from the table below:
`debug.startSectorEffect(CorrectSeasonGUID,19990093)`
> 5. Press Shift+F1 to close the console.
> 6. The sector effect should now match the current season quest.

  |Season|Summer|Autumn|Winter|Spring|
  |---|---|---|---|---|
  |GUID|19990307|19990378|19990370|19990374|
