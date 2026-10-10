<h1>Vendor Management System<img align="right" src="./Data/images/main.png" width="100px"></h1>

Nearly-fully automated vendor management system to allow players to run and operate shops that are setup by staff members. This vendor system even allows custom item categories to be setup (e.g. Armor, Potions, Spell Scrolls, etc.).

[Shadow's Main Website](https://shadow-draconic-development.github.io/.github/)

[Shadow's Discord Server](https://discord.gg/JqaH7Nbgmr)

## Help
An administrator must run `!shop setup [channel id]` in order to setup channels for vendors. If you run `!shop setup server`, you can setup a server-wide vendor.

After running this command, you must then run `!gvar editor [GVAR UUID] @person` in order to grant permissions for shop owners to actually edit the GVAR.

If you need to reference a GVAR in the future, you can run `!shop setup list` to list previously added GVARs.

Once the vendor has been setup, you can now add items to the vendors for people to buy.

- Channel-only vendors:
    - Simply run `!shop stock add [item name] [item cost] [item category]` in a designated channel or in a thread underneath a designated channel.
- Server-wide vendor:
    - Simply run `!shop stock add [item name] [item cost] [item category]` in any channel that is not designated as a channel-vendor.

You can view stock by running `!shop stock` or `!shop`. Players, at this point, may purchase items for sale by running `!shop [item name]`.

Removing stock works in a similar fashion as above.

- Channel-only vendors:
    - Simply run `!shop stock remove [item name] [item cost] [item category]` in a designated channel or in a thread underneath a designated channel.
- Server-wide vendor:
    - Simply run `!shop stock remove [item name] [item cost] [item category]` in any channel that is not designated as a channel-vendor.

To remove vendors from the server, an administrator can run `!shop setup remove [channel id]` to remove a channel-specific vendor. Or to remove the server vendor, run `!shop setup remove server`. **_MAKE SURE NOT TO DELETE CHANNELS YOU DO NOT INTEND ON REMOVING AS REMOVING CHANNEL/SERVER VENDORS CANNOT BE REVERSED_**

## FAQ
Q. **How do I get the IDs of the channels I want to setup?**

A. You need to enable developer mode. Follow Step 0 of [this documentation](https://docs.discord.com/developers/activities/building-an-activity#step-0-enable-developer-mode). Then do the following:

- On desktop, right click the channel you want and "Copy Channel ID" should be at the bottom of the drop down menu. 
- On mobile, tap and hold a channel you want and scroll to the bottom and "Copy Channel ID" should be at the bottom 

Q. **I keep on getting an error when trying to add/remove stock from a vendor. What do I need to do?**

A. You likely do not have editor permissions, talk to the administrator that setup your vendor and talk to them about running `!gvar editor [GVAR UUID] @you`.

Q. **Can you make it so that items get removed as people buy them?**

A. No I cannot, it would require administrators to run `!gvar editor [GVAR UUID] @person` on every person that uses the shop. Such would allow other players to alter item stock and there is no way to prevent misuse.

## License Notice
This work includes material written by Seth Hartman (aka ShadowsStride) and is licensed under the Creative Commons Attribution 4.0 International License available at https://creativecommons.org/licenses/by/4.0/legalcode.

## Requests
Requests can be made at this [link.](https://forms.gle/YYkyPcBb1WHXWMYE6)

All requests can be viewed at this [link.](https://docs.google.com/spreadsheets/d/1OyW78hh1ARDHeDu4hF4X2TxcpYSrrArprs8pkQB3zo4/edit?usp=sharing) All requests are viewable by all, if I have any problems I will restrict access to these links.

## Donations
You can click the button below to view my ko-fi and patreon page. Donations like this help me write more aliases and donators do get priority on feature requests.

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/F2F6MG4NH) [Patreon](https://www.patreon.com/bePatron?u=47388431)