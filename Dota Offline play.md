
Ever wondered how to play Dota 2 offlline without internet?
Tip
Start Steam in offline mode

Go to Library, right click on Dota 2, Properties, Set Launch Options

add command '-console'

Start the game

Open the console and write next:

dota_start_ai_game 1 sv_lan 1 sv_cheats 1 dota_bot_set_difficulty 0/1/2/3 -depends in against what bot difficulty you want to play against map dota


[Tip]How to play a single player game vs bots in Offline mode!
Tip
UPDATE 1 :- Sorry for the ambiguity in the title, but this is not a guide to play against bots sorry.

Okay I know not all of you guys have internet connection at all times or just wanna try new stuff vs practice bots, so here is the full tutorial.

First you have to enable -console in the launch options of Dota 2 in Steam settings. Just type "-console" without quotes in the text box of launch options (Default key for console is "`").

Then start Steam in Offline mode(not necessary but wouldn't hurt)

In the console which appears over the "Connecting to Dota 2 network" type the following commands, hitting enter after each one.

sv_cheats 1

sv_lan 1

dota_start_ai_game 1

dota_bot_set_difficulty 0/1/2/3 (For the true enthusiast :D )

or

dota_bot_practice_difficulty 0/1/2/3

map dota

4) You can also load the diretide/tutorial/winter/autumn maps, they will appear in a dropdown menu after you type "map dota"

5) Happy Practicing!



v2


Guide on how to play DotA 2 in Steam offline mode
Por 𝓑𝓸𝓷𝓮𝓣𝓸𝓪𝓭
If you want to play without bots you can just skip the plain text and follow the bold text only.

This is a guide on how to LAN Dota 2 when you're at friends etc. and have no internet connection. Normally Dota won't let you LAN only play bot matches solo in offline mode. This is for those people(like me) frustrated that you can't LAN Dota without internet connection.

1st
So to do this you'll need to enable console first by right clicking Dota 2 in steam and selecting "Properties". Then click on "Launch Options" and type in "-console". Click OK and close, you can start the game now and it should take you to something similiar to this screen.

Now type this in the console: "sv_cheats 1" "sv_lan 1" "map dota.bsp"

Once the map loads in the background and you can type in the console again, make a note of the server port in the console here . Your friends will be using this to connect to your game. Now if you want to play with bots type the following in the console: "dota_bot_set_difficulty 3". You can replace the 3 with numbers from 1-3. 1 being easy bots, 3 being hard bots(I am not sure on the difficulty ranking with the numbers maybe it goes from 0-4, 0 being passive and 4 being unfair but I just use 3 all the time anyways which I'm sure are hard bots). Now type "dota_start_ai_game 1". When all this is done, your friends can connect from their consoles by typing in "connect" and your private LAN IP address followed by the port your got earlier. Something like this "connect 192.168.10.12:27015".[/b] When your friends are connected, you and them pick Radiant or Dire side by typing in "jointeam good" for Radiant or "jointeam bad" for Dire and "jointeam spec" for spectator. Then close the console using the x at the top right or pressing the keybind for console. Pick heroes and the bots should load in once the game starts. This is a guide for playing All Pick only, if there is a way to play other gameomdes using console then post it in the comments.
2nd
Btw I know this is an unnecessarily long and in-depth guide just to type a few commands in the console, but I wanted to make this as noob-friendly as possible. Hopefully this helps some people like it did me.

To select the game mode, you have to type "dota_force_gamemode X" into console before "map dota". X is a number that defines the game mode you will play (Source: http://dota2.gamepedia.com/List_of_Console_Commands): * All Pick = 1 * Captains Mode = 2 * Random Draft = 3 * Single Draft = 4 * All Random = 5 * INTRO = 6 * Diretide = 7 * Reverse Captains Mode = 8 * Greeviling = 9 * Tutorial = 10 * Mid Only = 11 * Least Played = 12 * Limited Heroes = 13 * Compendium = 14 * Captains Draft = 16 * Balanced Draft = 17 * Ability Draft = 18 * All Random Death Match = 20 * 1 VS 1 Solo-Mid = 21 * All Pick (Ranked) = 22
3rd
Here are the list of commands I followed, Scenario: want to play with my friend over lan without internet.

[server]
sv_cheats 1
sv_lan 1
dota_bot_set_difficulty 4
dota_start_ai_game 1
dota_force_gamemode 1
map dota.bsp
jointeam good/bad
[client(s)]
connect IP:PORT
jointeam good/bad
[server]
dota_bot_populate
The dota_bot_populate command fills empty slots with bot heros