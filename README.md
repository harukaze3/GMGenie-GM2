# GMGenie-Duskhaven
GMGenie, modified by Haruka

Game Master Genie
=======


About GM Genie
-------

[![Screenshot of GM Genie](http://www.chocochaos.com/gmgenie/GMGenie%200.7.thumb.jpg)](http://chocochaos.com/gmgenie/GMGenie%200.7.jpg)

GM Genie is an all-round GM addon for TrinityCore, aimed at making common tasks easier and quicker to accomplish. It provides tools for managing tickets, interacting with players on the server, building/spawning and much much more.

Current Functionaility
-------

*   **Hud aka the main window**
     Shows the amount of open tickets, both online and offline. Shows gm status and allows changing it. And provides quick access to the ticket and builder interface.
*   **Tickets**
    May not sound all too interesting, but decent ticket addons are hard to find these days. This one is extra cool as it has some neat functionality, including but not limited to:
    *   Read marking: easily see which tickets have and have not yet been read.
    *   Differentiation between online and offline tickets, including the option to hide offline tickets if you wish.
    *   Sort by tickets by id, name, creation date, modified date or assigned to.
    *   Show who else is reading the ticket while you are reading it.
    *   Quickly assigning the ticket to yourself with a single click, or to someone else by right clicking.
    *   The ability to set comments from within the ticket window, instantly updating the comment if someone else has the ticket open as well.
    *   Fully integrated with the awesome spy (see below).
*   **Spy aka playerinfo**
    Spy is a window showing all relevant info from the usefull playerinfo command. In addition, it provides access to several quick commands, macros and advanced character tools. Spy is opened automatically when a ticket is opened, and can be initialized manually by typing /why charactername or by right clicking a name in chat, going to quick commands and clicking spy.
    *   Appear, summon, freeze, unfreeze, revive, rename, customize, change race, change class, etc.
    *   Lookup other accounts and characters from the player.
    *   Show any current or past bans.
    *   Quick ccess to all whisper, mail and discipline macros (see below).
*   **Player macros**
    There are three types of player macros: whisper macros (which send pre-defined whispers), mail macros (to send pre-defined mails) and discipline macros (for any kind of pre-defined mutes or bans).
    Macros can be easily defined from the interface settings. Each type comes with several neat options to customise the macros to your needs.
    The macros can be accessed from the spy window, and when right clicking a player in chat (or somewhere else, as long as there is normally a player menu on right click).
*   **Builder**
    The builder allows exact movement, rotation and spawning of npcs and objects. The combination of these two options make it a pretty powerful tool that can be used to make almost anything in-game.
    In addition there is also a window to make "spawn macros". Usage requires a basic understanding of lua. A few examples:
    *   A cirlce with 18 chairs:
    
            for i=1, 18, 1 do
            go(5, 0, 0, 180, -1, 1, 176232);
            go(5, 0, 0, 200, -1, 0, 0);
            end
            
    *   A spiral of torches going up:
    
            for i=1, 400, 1 do
            local rotate = 2+0.05*(2.71828183^(0.0125*i))
            local up = rotate/100;
            go(0.25, 0, up, rotate, -1, 1, 180352);
            end
            
    An example of what can be accomplished once you are familiar with the builder:
    [http://www.youtube.com/watch?v=A_4r1vEJ3MQ](http://www.youtube.com/watch?v=A_4r1vEJ3MQ)

The above certainly isn't a complete list of what the addon can do, but there's no point making a wall of text that no one will read anyway. I'd highly encourage just testing some things out and see what it can do for you. If you know lua, a peek at the source code may also shed some light on the functionality.

The addon is released under the GPL (v3), so feel free to modify, redistribute or whatever you'd like to do with it. If you find any bugs, have ideas for improvements, want to provide a patch or whatever, please feel free to post it here.



Reposts and modifications
-------

Since GM Genie is under an open source license, any modifications and redistributions of the addon are explicitely allowed, as long as copyright and license notices remain intact.

However, I would appreciate it if you could drop me a message if you post/publish GM Genie somewhere. Partly because I like to know where it is being spread, but also so I can add new versions to those threads when they are released. It would be a shame if everyone keeps using some ancient version because it was once posted on a forum, and never updated there.

You can drop me an e-mail at gmgenie [at] chocochaos [dot] com

It's not a requirement to inform me, but I would appreciate it =)



Changelog
-------

### Version 0.9.0
*   Duskhaven-side Ownership force-transferred to Haruka
    - Added a Close button
	-	.ticket close
    - All previous functions stayed the same
