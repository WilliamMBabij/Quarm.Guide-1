---
date: 2024-09-01T00:00:00.000Z
title: Zeal Readme
description: Readme for Zeal
keywords: 'Project Quarm, Quarm, EverQuest, crash fixes, Zeal, '
author: Salty
published: true
sitemap: true
---
## Zeal Readme 9-01-2024

Zeal pipes in c#

    https://github.com/OkieDan/ZealPipes

Compatible UI's

    https://github.com/NilliP/NillipussUI_1080p
    https://github.com/NilliP/NillipussUI_1440p
    https://www.eqinterface.com/downloads/fileinfo.php?id=6959

Features

    Camera motion improvements
    Additional binds
    Additional commands
    Additional ui support
    Various bug fixes
    Unique npc naming for better parsing

% Replacements

    %n or %mana for mana%
    %h or %hp for hp%
    %loc for your location
    %th or %targethp for your targets health %

Commands
    /autofire
        Description Toggles Autofire on and off. When you throw or shoot you will automatically continue to throw or shoot on cooldown.
    /cc
        Arguments: ``
        Example: /cc
        Description: toggles classic classes in who and other areas.

    /targetring
        Arguments: size, indicator
        Example: /targetring 0.25
        Example: /targetring indicator toggles auto attack indicator.
        Description: toggles targetring on/off.

    /resetexp
        Arguments: ``
        Example: /resetexp
        Description: resets the exp per hour calculations.

    /timer
        Arguments: int
        Example: /timer 10
        Description: holds the last hotbutton pressed down for the duration (decisecond like /pause).

    /pipedelay
        Arguments: int
        Example: /pipedelay 500
        Description: changes the delay between each loop of labels/gauges being sent out over the named pipe.

    /pipe
        Arguments: string
        Example: /pipe set a respawn timer for 30 seconds
        Description: outputs a string through the named pipe.

    /ttimer
        Arguments: int
        Example: /ttimer 500
        Description: change the delay in which a tooltip pops up on mouse hover.

    /inspect target
        Description: adds target argument to /inspect, this just inspects your current target.

    /loc noprint
        Description: adds noprint argument to /loc, this just sends loc directly to your log.

    /reloadskin
        Description: reloads your current skin using ini.

    /fov
        Arguments: int
        Example: /fov 65
        Description: changes your field of view with a value between 45 and 90.

    /melody
        Arguments: song gem #'s (maximum of 5)
        Aliases: /mel
        Example: /melody 1 4 2 3
        Description: plays songs in order until interrupted in any fashion.

    /map
        Arguments: on, off, rect, marker, background, zoom, poi
        Example: /map toggles map on and off
        Example: /map marker 500 -100 sets a target marker at loc 500, -100 (default size)
        Example: /map marker 500 -100 3 sets a target marker at loc 500, -100 with size = 3% of screen
        Example: /map 500 -100 shortcut for map marker 500 -100
        Example: /map 0 shortcut for map marker 0 0 0 (clears marker)
        Example: /map zoom 200 sets map scaling to 200% (2x) and centers on position
        Example: /map rect 2 3 50 60 map window top=2% left=3% bottom=50% right=60% of screen dimensions
        Example: /map poi lists points of interest, use /map poi 2 to drop marker at index [2] of list
        Description: controls map enable, size, and markers

    /pandelay
        Arguments: ms delay, none
        Example: /pandelay 200
        Description: changes the amount of delay before left click panning will start to happen

    /hidecorpse
        Arguments: looted, none
        Aliases: /hideco, /hidec, /hc
        Example: /hidecorpse looted
        Description: looted Hides a corpse after you have looted it., none reveals all hidden corpses

    /spellset
        Arguments: save, load, delete
        Example: /spellset save buffs
        Example: /spellset load buffs
        Example: /spellset delete buffs
        Description: allows you to save and load spellsets

    /showhelm
        Aliases: /helm
        Arguments: on, off
        Example: /showhelm on
        Description: Toggles your helmet.

    /showlootlockouts
        Aliases: /showlootlockout, /showlockout, /sll
        Description: Shows you your current loot lockouts on Quarm.

    /zealcam
        Aliases: /smoothing
        Arguments: x y 3rdperson_x 3rdperson_y
        Example: /zealcam 0.7 0.2 0.7 0.2 if 3rd person arguments are not supplied, the first x and y are applied to both
        Description: Toggles Zeal's mouse look smoothing methods, the first 2 arguments are first person sensitivity, and the last 2 are for 3rd person

    /autoinventory
        Aliases: /autoinv, /ai
        Description: Drops whatever is on your cursor into your inventory.

    /autobank
        Aliases: /autoba, /ab
        Description: Drops whatever is on your cursor into your bank. [requires you to be at a banker] (not fully functional atm)

    /target
        Aliases: /cleartarget
        Description: acts as normal /target unless you provide no argument in which case it will clear your target.

    /sit
        Description: The /sit command now accepts "on" as an argument. Using "/sit on" will always make you sit, even if you are currently sitting. This matches the game's native "/sit off" which always makes you stand even if you are currently standing. The "/sit" command will continue to toggle sit/stand state if no argument is provided or if the argument provided is not on or off. Additionally, "/sit down" now works as well and will always make you sit, even if already sitting.

    /camp
        Description: Auto sits before camping.

    /zeal
        Arguments: version
        Description: Shows the version of zeal.

    /zealinput
        Description: toggles the zeal input setup for any input in game, giving you a more modern input (ctrl+c, ctrl+v, left, right, shift left+right for highlighting, home, end ect).

    /help zeal
        Description: Shows the custom Zeal commands.

    /timestamp
        Aliases: /tms
        Description: Shows message timestamps.

    /outputfile
        Aliases: /output, /out
        Arguments: inventory | spellbook [optional_name]
        Example: /outputfile inventory my_inventory
        Description:
            inventory outputs information about your equipment, inventory bag slots, held item, and bank slots to a file.
            spellbook outputs a list of all spell ids current scribed in your spellbook.

    /buffs
        Description: Outputs the players buff timers to the chat only if they are using OldUI.

    /bluecon
        Description: Changes the blue con color to usercolor #70 which is otherwise unused, you can edit in the options window.

    /alarm
        Arguments: oldui
        Description: Re-opens the alarm window, if oldui is specified it allows for an alarm on it.

Binds

    Cycle through nearest NPCs
    Cycle through nearest PCs
    Strafe Right
    Strafe Left
    Auto Inventory
    Toggle last 2 targets
    Reply target
    Pet Attack
    Pet Guard
    Pet Follow
    Pet Back
    Slow turn left
    Slow turn right
    Target nearest pc corpse
    Target nearest npc corpse
    Toggle map on/off
    Toggle through map default zooms
    Toggle through map backgrounds

UI

    Gauge EqType's
        23 EXP Per Hour

    Label EqType's
        80 Mana/Max Mana
        81 Exp Per Hour Percentage
        124 Current Mana
        125 Max Mana
        134 Spell being casted

    LootAllButton

    LinkAllButton

Options UI

    ScreenID Checkboxes
        Zeal_ShowHelm
        Zeal_HideCorpse
        Zeal_Cam
        Zeal_BlueCon
        Zeal_Timestamp
        Zeal_Input
        Zeal_Escape_

    ScreenID Sliders
        Zeal_PanDelaySlider
        Zeal_FirstPersonSlider_X
        Zeal_FirstPersonSlider_Y
        Zeal_ThirdPersonSlider_X
        Zeal_ThirdPersonSlider_Y

    ScreenID Labels
        Zeal_ThirdPersonLabel_X
        Zeal_ThirdPersonLabel_Y
        Zeal_FirstPersonLabel_X
        Zeal_FirstPersonLabel_Y
        Zeal_PanDelayLabel

Building
Github official release builds

    Commit an updated, unique ZEAL_VERSION in Zeal/Zeal.h that will be used as the release tag.
    Go to the "Actions" tab of the Github workspace
    Select the "Create Manual Release" workflow on the left
    Click the drop-down menu on the right top side titled "Run workflow"
    Select the branch with the commit to be released
    Add a summary description that will be prepended to the change log notes
    Click the green "Run workflow" button
    After the green checkmark appears, go back to the main workspace and verify the content of the new release tag.

Local builds

Build in 32bit x86 mode using Microsoft Visual Studio 2022 (free Community edition works)
Installation

    Download the "zeal_v*.zip" from a tagged release on github
    Extract zeal.asi and place it in the root of your game folder
    Extract EQUI_OptionsWindow.xml and place it in your active ui folder (example: uifiles/duxaUI)

The zeal.pdb file is a symbols file only useful for debugging with developer tools (ignore).

file extension .asi
<br>
move zeal.asi into the root of your game folder

