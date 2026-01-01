# SecretEPGP
Guild Helper addon for EPGP loot system in WoW (1.12)
This has the adjusted pricing for Secret Hideout.

## Setup
SecretEPGP requires some modifications to guild permissions for officer notes by the guild leader.  

### Version 3.x (current)
- officer notes must be set to visible by all and editable **only** by the EPGP admins (eg. officer rank+)
- public notes are not in use by the addon

## Tips
Create a new chatframe (right-click > create new window on chat tab) and name it `debug` (capitalization doesn't matter)  
Most of the information messages will now print on that frame and not clutter your default chatframe.

## Usage
Right-click on minimap or FuBar SecretEPGP icon will show all available settings.  
Left-click shows the standings window with everyone's EP, GP and PR values. 
The standings window can also be toggled with **/shooty show** chat command. 

## Features
- EPGP standings list (all)
- Simple chatlink click to bid on items (all)
- Item Bids list (admin/ML)
- Item GP prices on item tooltips (all)
- Export standings to csv (all)
- Configurable EPGP Decay (admin)
- Configurable Offspec discount (admin)
- Guild Progression multiplier (admin)
- Reserves - *standby list EP* - with alts support (admin and all)

Addon has been designed so that basic member functionality is usable even without the addon. 
- `/w <masterlooter name> +` (for main spec) or `/w <masterlooter name> -` (for off spec) after the loot officer links a piece of loot and asks for bids in raid chat.  
- Type `/x +` (where x is the number of the custom channel) or `/x +MainName` if on an alt to respond to a standby list afk check.  
Having the addon makes everything more convenient, but is not mandatory.

## EPGP basics and help
[SecretEPGP wiki](https://github.com/Road-block/SecretEPGP/wiki)

## Key Points about Secret Hideout EPGP

### Pricing and Item Value:
Item prices vary based on their importance. Best-in-slot (BiS) items are priced higher due to their long-term value, while minor upgrades are priced lower. Factors affecting pricing may evolve as we gain experience with the system.

### How to Bid on Items:
During raids, items will be posted in raid warnings. If interested, whisper “+” for main spec (MS) or “-” for off spec (OS). 
MS bids always take priority over OS bids.
You can attempt to save points by bidding OS, but others may have a higher Priority Rating (PR). As with an auction, lower bids risk losing the item.
The Master Looter will announce when the bidding period is about to close. Items are awarded first to the highest PR among MS bids, then to OS bids.

### No Bids:
If no one bids on an item, it will go to a free roll for all eligible players who can equip it, including those rolling for transmog. All interested raid members should /roll, and the item will be given to the highest roll. Guild members are prohibited from rolling solely to sell items. Unwanted items will be disenchanted.

### Allowed Bidders:
Only main characters can bid for main spec (MS). This prevents alts from competing with mains for MS items. Off spec (OS) bids from mains and alts are treated equally.
If a main character allows an item to go to OS, they risk losing it to another OS bid, including from an alt. No exceptions will be made.
It is the responsibility of main players to place an MS bid if they want an item for their main spec.

### Checking Your PR:
Calculate PR by dividing your EP (Effort Points) by your GP (Gear Points), as shown in your Officer Note in-game. 
Example: Woodbender has 100 EP and 100 GP, resulting in a PR of 1. Bapi has 335 EP and 100 GP, resulting in a PR of 3.35. If both bid, Bapi wins due to the higher PR.
Handling Ties:
In the event of a tie in PR for the same item, the tied players will roll to determine the winner. This should become less frequent as the system stabilizes.

### Decay for EP and GP:
Decay ensures fairness by prioritizing recent contributions. At regular intervals (e.g., weekly), a percentage of EP and GP decays. 
Example: With 10% decay, 1000 EP and 500 GP would reduce by 100 EP and 50 GP. PR adjusts automatically.
Details about decay rates and schedules will be shared.
Decay is currently set at 10%, but may be adjusted as the Officers feel necessary.

### EPGP Addon:
The EPGP addon is not mandatory for raid members, except for the Loot Master. However, if you choose to use it, the addon will automatically display the assigned item values in Atlas for your convenience.