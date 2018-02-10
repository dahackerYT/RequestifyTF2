# RequestifyTF2
![Build](https://ci.appveyor.com/api/projects/status/github/weespin/Requestifytf2)

RequesifyTF2 is a simple program for Source Engine based games, which supports plugins. "Oof" killmicspam supported!
# Installation
1. Go to Download and download lastest [releases](https://github.com/weespin/RequestifyTF2/releases)!
2. Make sure that you have [Virtual Audio Cable (paid)](http://software.muzychenko.net/eng/vac.htm) or [VB-Audio (free)](http://vbaudio.jcedeveloppement.com/Download_CABLE/VBCABLE_Driver_Pack43.zip) installed on your pc
3. Open RequestifyTF2
4. Press on Settings button
5. Select path to the game (for example C:\(something)\steamapps\common\Team Fortress 2\tf or C:\(something)\steamapps\common\Counter-Strike Global Offensive\csgo)
6. Press Start button (you should press start before starting a game!)
7. Make sure you have a Virtual Audio Cable or VB-Audio recording device for default.
8. Start your game!
9. When you joined a server open console and type "+voicerecord"
10. If you want to hear what you saying type "voice_loopback 1"
11. Done!
# Another plugins
I have released some plugins but i don't want to include them into default version, so please look at [Plugins page](https://ci.appveyor.com/project/weespin26279/requestifytf2/build/artifacts) and download needed plugin.
# Updating
If new version was released, just replace RequestifyTF2GUI.exe with new file, and remove plugins!
# Screenshots
![Plugins](http://i.imgur.com/ccoM7Dy.png)

![Ignore List](http://i.imgur.com/T2cVaVE.png)

![Settings + Console](http://i.imgur.com/zv2sd03.png)
# Old Screenshots
![Old](http://i.imgur.com/J2XXlDS.png)

![Old1](http://i.imgur.com/Xx9lJph.png)

# Dowload
[Releases](https://github.com/weespin/RequestifyTF2/releases)!
(Download RequestifyTF2GUI.exe)
## Bleeding Edge files
[Download](https://ci.appveyor.com/project/weespin26279/requestifytf2/build/artifacts)
# About Valve Anti-Cheat (VAC)
## This programm is not a hack, not a cheat, not modifying game files, not injecting into game processes, not reading and writing into games memory.
My programm is 100% VAC secure, its not even reading game memory!
Its reading 1 file named console.log which was generated by game using in game console command con_logfile "console.log"

Game is writing log from console into a file and im reading this log as text file. Thats all!

[This programm can work with AHK. But AHK is not used now.](https://gaming.stackexchange.com/a/301540)
# Plugin Requesting
Be free to create a issue and write idea about next plugin.
Requestify can do something:
 1. On calling command
 2. On text chatting
 3. On killing
 4. On suiciding
 5. On another players connect
 6. Do config commands (with generated code)
# Development
## Core
Download RequestifyTF2.dll from [AppVeyor](https://ci.appveyor.com/project/weespin26279/requestifytf2/build/artifacts) (RequestifyTF2.dll)
## Template
Just use a plugins from scr/Plugin folder as tempate.
# Methods
## OnLoad (should be non-static!)
Invokes on Load
## Execute (string nickname, List<string> arguments)
Invokes when someone executed a plugins command
# Events
OnPlayerConnect => Returns a connected user nickname

OnPlayerChat => Returns a user nickname and text (invoked if text is not a command!)

OnPlayerKill => Returns Killer's Nickname, Killed Nickname, Weapon and crit (TF2 only)

OnPlayerSuicide => Returns a user nickname (TF2 only)
# Questions?
Make a issue or add me on [Steam](http://steamcommunity.com/id/wspin/)
