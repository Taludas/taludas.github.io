# The Wholesome Hacienda Haul

<div align=center><img src="_media/Anno1800/mod_banners/haciendaoverhaul/Thumbnail.png"/></div>

<div align=center><a href="https://github.com/Taludas/WholesomeHaciendaHaul/releases/latest/download/WholesomeHaciendaHaul.zip"> <font size="40">Download now</font></a></div>

This is a modular overhaul of the DLC10 Seeds of Change which touches nearly every aspect of newly introduced gameplay into the sandbox mod. Pick and choose which changes you like the most!

If you like this mod and want to support me, feel free to share it with your friends. You can also buy me a coffee at Ko-Fi!

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/W7W8L558T)

## How to use

- Automatic install using the Anno Mod Browser, available from the main menu of your Anno 1800 game.
- Either use [iModYourAnno](https://github.com/anno-mods/iModYourAnno/releases) mod manager or know [how to install mods manually](https://github.com/jakobharder/anno1800-mod-loader#mods).
- If you download the mod manually, use the archive from [GitHub releases](https://github.com/Taludas/WholesomeHaciendaHaul/releases). Don't download the whole repo!

**If you change from versions 1.x.x to version 2.0, it is extremely important to remove all older versions of this mod. The Mod is now a single mod folder and modules are disabled through editing assets.xml file or through IModYourAnno Mod Manager! If you use iModYourAnno, please notice, that you have to turn on all toggles in the Tweaking tab to get the intended 'Full Experience'!**

## Features

This is my version of DLC10 Seeds of Change as I have envisioned it to be from the first moment I saw gameplay. Unfortunately the initial release left me and many other members of the community behind their expectations. I conducted a research of the most wanted changes and modded it into the game. This is the list of features:

### New separate build menu for all Hacienda buildings
I created a separate build menu entry dedicated to only Hacienda buildings. Everything can be build from there.

### New Icons for all Hacienda Modules for easier identification and accessibility
The Icons of the Hacienda Modules lack distinctive features and contrast, it is really hard to tell them apart. So everyone got a new and distinct looking icon.

### Hacienda Streets now unlimited and working like normal streets
The Hacienda Streets have been limited to 999 tiles combined for an unknown reason. No longer! Each module is now separate and works like a normal street. They can now be built over Rivers and Train Tracks as well. (Thank you to Muggenstuermer's ["City Ornaments"](https://www.nexusmods.com/anno1800/mods/93?tab=description)).

### Radius of the Hacienda now up to 80
I increased the maximum range to 80 starting at 15. To give an extra incentive to build population inside the Hacienda radius, the last two steps are reserved for hitting 7500 and 10000 population (+5 on the radius each time). To accommodate the new radius, the distance over which the Hacienda provides its Public Service to houses has been increased as well. You should be able to easily fit residences at the outer parts of the radius if using paved streets (or Hacienda Plaza). This feature is fully tweakable through iModYourAnno.

### Hacienda Warehouse now up to 100 tons of storage and one transporter
The vanilla Hacienda Warehouse hasn’t a real value over the normal Depots inside the harbour area, as they even use up precious land space. So I gave them a new task with adding one transporter ramp to them and increasing the storage space to 100 tons. This comes at a cost though. The can only be build inside the Hacienda radius and they’ll cost you 50 Obrero Workforce each! They should only act as a support to regular warehouses. This feature is fully tweakable through iModYourAnno.

### Hacienda residences have been overhauled completely
- Jornalero residences now take up to 85 Population each with lifestyle needs. Their needs have been left unchanged, but an extra incentive has been given to the two new goods Schnaps and Hot Sauce by increasing the amount of gained inhabitants.
- The next big change is that Obrero residences can’t be build separately any longer. You’ll need to upgrade your Jornalero residences.
- For the Obrero Residences, they now get 3 points of attractiveness by default to help you reach the required amounts of it to unlock the Hacienda policies. Their inhabitant count has been lifted to 165. An extra incentive was given to the new products Hot Sauce and Atole as well as the newly introduced needs: Chewing Gum and Violins unlocked at 1500 and 2000 Obreros respectively to further strengthen the incentive to build those production lines in later game.
- To accommodate the changed needs, population boosting items like Saint D’Artois and Papal Paper now give extra residents from Hot Sauce as well as Chewing gums and Violins to promote not only NW usage of these goods but also the supply of Violins and Chewing gum to Engineer and Investor Skyscrapers, as those productions are not really space efficient for the amount of inhabitants they give.

### Fertilizer Factory got buffed and hasn’t to be build inside the Hacienda Radius
Production time of the Fertilizer Factory has been lifted to 90 seconds. At the same time, the buff for the animal farms has been reduced to 1/10 instead of 1/3. Now you have to build 3 Animal farms at 110% to supply one unboosted Fertilizer Factory instead of a one to three ratio as before. The Fertilizer Factory also doesn’t need to be build inside the Hacienda radius any more, because I think most of us don’t wanna wake to the smell of poop every day, would we?

### Hacienda Farms: 4 new crop types and fertilities mater again
Why exactly is it that the Devs left out the three crops Bananas, Cotton and Tobacco? Well, I theorize that the recipe book has no more space than to fit 8 recipes at the current scale of each item on the list. So they told their art team to design all crop farms for the New World fertilities and then dumped the ones nobody likes - because of balancing and item game - overboard. But the graphics did survive the drip into the final game files! I spent an hour creating the Tobacco plantation until I noticed at export that there already is on! I mean wtf. I paid full price but due to a really simple UI design problem, so much content was stolen from me. Especially since the Tobacco Plantation was one of the most unused Farm in the entire game, a Hacienda version in vanilla could have made a really good opportunity to actually plant it instead of getting it as a by-product from bananas.

- So, I fixed that issue myself with a split of hacienda crop farms into two buildings, New World Hacienda Crop Farms including the long lost Banana, Cotton and Tobacco Plantations and OW Hacienda Crop Farms plus spices and *drum role please* a Vineyard! More on that later. With update 2.2.0 we also have the missing Farms from DLC12: Herbs and Orchids!

- The recipe books are now split as well, so watch out for that. All farms have been checked for their production time to fit vanilla. Since the importance of the Hot Sauce is increased drastically, Spice Farm production cycle was set to 120 seconds, so that supply becomes a bit more of a challenge. Another big change is that all New World Crop Farms and the Vineyard now require the corresponding fertility on the island. I don’t get it why such an old feature of the Anno series should now be dropped entirely.

- Farms and recipes are now locked to begin with. Now more Cocoa or Coffee Plantations if your residents don’t require the appropriate finished Product. This should ease the new player starting with a new savegame to have a little bit of visible progress.

- Hacienda Breweries: checked and adjusted. I adjusted the negative impact on Attractiveness by Hacienda Breweries to +5 to help with the unlock of all Hacienda policies. The building costs were raised to 10 Timber and 15 Bricks. The production time of the Hot Sauce Brewery was lowered to 60 seconds for above stated reasons of balancing the newly popular need vs the amount of pop you get from it. Breweries and their recipes are now locked to begin with. Now more Atole or Coffee if your residents don’t require the appropriate product. This should ease the new player starting with a new savegame to have a little bit of visible progress.

### Support for most important Public Buildings to use the Hacienda Plaza ground decal
This one is for the beauty builders in the Community. I took every major public building and gave them a new variation with the Hacienda Plaza ground decal, so that you can build magnificent Hacienda Compounds with fitting Public Buildings.

Included are: Firestation, Police Station, Hospital, Chapel, Boxing Arena and all Warehouses as well as the DLC12 public buildings.

### Hacienda Policies completely replaced and rebalanced
To be honest the vanilla Policies are like playing with the small scoops in Kindergarden while the bigger kids got the nice Tractors and Earthmovers. In comparison to the Palace buffs, they look nearly useless. For the fourth one you have to pay nearly the same amount into Attractiveness enhancement to break even. That’s no good game design. The Buffs from the Scenario Hacienda are way more powerful and would have fitted as well.

But as I’m more creative than that, I created 5 totally new and potentially game changing buffs for you to play around with. Now you’ll definitely consider every one of them.

- Decree 1: Clean Environment Regulation (required Attractiveness: 450)
    * Effects All Heavy Industries, all Mines, all Quarries, all NW Chemical Plants and all Breweries:
        * Productivity +20%
        * Chance of Fire -50%
        * Chance of Explosion -100%
        * Negative Infliction on Attractiveness -80%
        * Workforce needed +25%
        * Maintenance Costs +75%

- Decree 2: Local Factory Outlet Regulation (required Attractiveness: 700)
    * Effects All New World Residences:
        - Reduced Consumption of:
            - Ponchos -25%
            - Bombins-15%
            - Coffee -10%
            - Cigars -10%
            - Fans -10%
            - Scooters -10%
        - Extra happiness from Market/Hacienda +5
        - Income -10%

    * Effects All Clothing Factories, all Intermediate Good Producers, Coffee Roaster, Cigar Factory, Fan Factory and Scooter Factory:
        * Extra Goods every third Cycle (1/3)
        * Attractiveness +5%
        * Workforce needed +15%
        * Maintenance Costs -50%

- Decree 3: Lumberjack Educational Decree (required Attractiveness: 1000)
    * Effects All Lumberjacks and all NW Orchards
        * Productivity +15%
        * Attractiveness +10
        * Workforce needed -50%
        * Forest Density -25%
        * Extra Goods: Wanza Wood 1/7 and Cherry Wood 1/10

- Decree 4: Vineyard Promotion Act (required Attractiveness: 1750)
    * Effects Hacienda Vineyards
        * Extra Grapes every second cycle (+50%)
        * Grape fertility provided
        * +25 Attractiveness

    * Effects Hacienda Winery
        * Extra Champagne every second cycle (+50%)
        * +25 Attractiveness

    * Effects all Artista residences:
        * +58 extra Money , +5 Happiness and +5 Inhabitants from the Champagne lifestyle need as well as a -25% reduction of said need.

- Decree 5: Cultural Conservation Act (required Attractiveness: 2200)
    * Effects all Obrero and all Artista Residences
        * Income per House -25%
        * Bonus Happiness +5 and Bonus Inhabitants +5 from Samba School and Lanterns
        * Reduced consumption of Light Bulbs (-25%), Fans (-50%) and Scooters (-75%)
        * Increased consumption of Typewriters (+25%), Soccer Balls (+50%) and Sewing Machines (+75%)
        * If the Boxing Arena need is fullfiled, the residences gain Cinema need fullfiled
        * If Lantern need is fullfiled, the residences gain Electricity need fullfiled

### Extended Hacienda by Lordys and Taludas
In cooperation with Lordys, I developed an extension to the Hacienda DLC with new public buildings, new 2x3 Hacienda residences and a outer Hacienda wall ornament to further customize your Gameplay experience.
* Small Marketstands → Satisfy need of Hacienda for Residences in its range
* Small Jornalero, Obrero Residences and Artista Residences (2x3) → 24/\[30\], 44/\[55\] and 68/\[85\] pop
* Hacienda Chapel → Satisfies Chapel Need
* Hacienda Fire Station, Hacienda Police Station (both with advanced Versions as well) → Two resolver units each and slightly higher coverage
* Hacienda Trade Union → Radius 20! Costs 50 Obrero Workforce though
* Hacienda Townhall
* Hacienda Border Wall Semi-Automatic and manual → read below!
* One quick word on the topic of the semi-automatic outer wall. Since the Anno Code only allows for ornaments to be in the middle of the decal to snap automatically into the right place, I had to use a trick. You have to build a two tile wide corridor of wall first. Afterwards you can safely delete the inner circle and the outer one will stay connected the right way!

### Mod Tweaks through iModYourAnno

If you use the [iModYourAnno Anno Mod Manager](https://github.com/anno-mods/iModYourAnno) you will find a tweaking tab in it. There are several options to tweak some gameplay elements of this mod. For example you can toggle whether the Hacienda Farms require a fertility. Or what recipe the winery uses. With regards to the policies you can decide to either use the vanilla ones or my modded ones and you can specify the required Attractiveness amount needed to unlock these. If you want the full experience, I suggest you switch every toggle option to 'on'. The value tweaking is up to your own liking. Feel free to experiment with your own numbers. Always remember to save you changes and delete the Cache Folder inside your mods folder afterwards.

### Bugfixes
- Hacienda Main Building removed from the ItemEffectTargetPool “All Hacienda Buildings” so that it can’t be boosted by Items which affect “All Production Buildings”.
- Hacienda Warehouse removed from the ItemEffectTargetPool “All Hacienda Buildings” so that it can’t be boosted by Items which affect “All Production Buildings”.
- Fixed a LOD issue with two of three Obrero Hacienda Residences: On one building side,suddenly windows appeared where none were visible before (LOD levels 2 and up)

### Acknowledgements
All that is left now, is to say thank you Ubisoft Mainz for a great game which I learned to love over the last 3 Years, that got me into some programming territory and self education about 3D Modelling as well as some amazing people on the Anno Mod Corner International Discord without whom this mod would have not been possible.

Special thanks to:
* Taubenangriff: For being a walking Lexikon for Anno Game Code knowledge and feedback and development of the IModYourAnno Mod Manager
* Jakob: For helping me with my very first modding attempts and developing the VSCode Plugin Anno Modding Tools as well as a Texture Converter and development of the IModYourAnno Mod Manager
* Lordys: Without whom I wouldn’t have ever been able to wrap my head around the function of the 3D game files and his amazing [Blender cfg Import/Export Addon](https://github.com/xormenter/Blender-Anno-.cfg-Import-Addon), he contributed all the buildings for the Hacienda Extended Module! THANK YOU :)
* JJE1000, Hackner and Pine: For feedback and constructive talks about features
* Meow for the amazing Mod Loader without this nothing of this would be possible
* lukts30: rdm4 converter
* VladiwSokow: for the idea of boosted transporters in the Arctic and how to do it

If you've read up to this point: What'll come next you ask... I plan on having a modular setup ontop of this base mod. For now only the working titles will be spoiled though:
* Module 1: The Burrito Boom (Done)
* Module 2: The Formidable Faulproof Fertiliser -TBD-
* Module 3: Willis Wine World-Tour (Done! -> Hacienda Winery)
* Module 4: The Mutile Mine Makeover (Done! -> Small Mods collection 'Mine Slot Unification')
* Module 5: Sweet, salty, sour or spicy? -TBD-
* Module 6: The Sounds  of Stradivari (Done! -> Violins in the Hacienda Build Menu)
* Module 7: The Cinematic Century Dawns -TBD-

That’s all! Hope you enjoy and happy city building!