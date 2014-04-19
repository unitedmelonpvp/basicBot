basicBot
========

Usage
-----

Bookmark the following code. To run the bot, run the bookmark.

javascript:$.getScript('dummylink');

###Special settings###

Standard settings can be used. Both the default settings and an example of a custom settings file (uses the .json extension) are included.
To use a settings file, make a public url for it. An easy way to do this is to upload it to dropbox and get a public link to it.
Include the link (for example www.mysettings.com/settings.json ) like this in your room's description, followed by a space or an enter:

@basicBot=www.mysettings.com/settings.json


Copyright
---------

Copyright &copy; 2012-2014 Thomas "TAT" Andresen and other contributors

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see http://www.gnu.org/licenses/.


Disclaimer
----------

This bot is developed independently. Changes may be made without notice. There is no guarantee for the perfect functioning.
Plug.dj admins have the right to request changes. 
By using this chatbot you agree to not use it for violating plug.dj's Terms of Service. 
You also agree not to alter the bot's code. Any requests for changes can be requested via email, through github or via plug.dj.


###Bot features (all can be disabled or enabled through commands)###

- data gets saved: upon refreshing the page the bot's data is saved up to 1 hour after refreshing
- dclookup: when a user leaves or disconnects, he/she can get his/her spot back when reconnecting within the specified time limit
- afk check: users that are afk (this is, not chatting: chats containing only a . or another symbol don't count), get automatically warned and removed after 2 warnings
- bouncer+: when enabled bouncers have extra permissions, like moving people in the waitlist
- mute: mute or unmute people
- cycleguard: disable DJ cycle waitlist if it's enabled too long
- lockguard: unlock the waitlist if it's locked for too long
- timeguard: skip songs that are too long
- MotD, Message of the Day: an optional message that is displayed every few songs
- links to facebook, youtube, a website... can be set using special bot settings

basic plug.dj bot
=================

Will be released in a few hours.

----------
DISCLAIMER
----------
This bot is developed independently. Changes may be made without notice. 
Plug.dj admins have the right to request changes. 
By using this chatbot you agree to not use it for violating plug.dj's Terms of Service. 
You also agree not to alter it's code. Any requests for changes can be requested via email, through github or via plug.dj.

---------------------------------------------------------------
Bot features (all can be disabled or enabled through commands):
---------------------------------------------------------------
- data gets saved: upon refreshing the page the bot's data is saved up to 1 hour after refreshing
- dclookup: when a user leaves or disconnects, he/she can get his/her spot back when reconnecting within the specified time limit
- afk check: users that are afk (this is, not chatting: chats containing only a . or another symbol don't count), get automatically warned and removed after 2 warnings
- bouncer+: when enabled bouncers have extra permissions, like moving people in the waitlist
- mute: mute or unmute people
- cycleguard: disable DJ cycle waitlist if it's enabled too long
- lockguard: unlock the waitlist if it's locked for too long
- timeguard: skip songs that are too long
- MotD, Message of the Day: an optional message that is displayed every few songs


---------
Commands:
---------

!command ---- arguments ---- description

arguments between ( ) are optional


Manager
-------

- !afklimit ---- X --- sets the maximum afk time
- !clearchat ---- ---- clears the chat
- !cycle ---- ---- toggle DJ cycle
- !cycletimer ---- X ---- set the maximum DJ cycle time for when cycleguard is enabled
- !locktimer ---- X ---- set the maximum time the waitlist can be locked if lockguard is enabled
- !refresh ---- ---- refreshes the browser of whoever runs the bot
- !usercmdcd ---- X ---- set the cooldown on commands by grey users
- !usercommands ---- ---- toggle user commands

Bouncer+
--------

- !add ---- @user ---- add user to the waitlist
- !autoskip ---- ---- skips songs automatically when they're done (use when the circles-bug happens)
- !bouncer+ ---- ---- disable bouncer+
- !lock ---- ---- lock the waitlist
- !lockdown ---- ---- lock down the room: only staff can chat
- !maxlength ---- X ---- specify the maximum length a song can be when timeguard is enabled
- !move ---- @user (X) ---- moves user to position X on the waitlist, default is position 1
- !remove ---- @user ---- remove user from the waitlist
- !unlock ---- ---- unlock the waitlist

Bouncer
-------

- !active ---- (X) ---- shows how many users chatted in the past X minutes. If no X specified, 60 is set as default
- !afkremoval ---- ---- toggles the afk check
- !afkreset ---- @user ---- resets the afk time of user
- !afktime ---- @user ---- shows how long user has been afk
- !ban ---- @user ---- bans user for 1 day
- !cycleguard ---- ---- toggles the cycleguard
- !dclookup ---- (@user) ---- do dclookup for user
- !english ---- @user ---- ask user to speak english (asked in the language they set plug to)
- !eta ---- (@user) ---- shows when user will reach the booth
- !filter ---- ---- toggles the chat filter
- !jointime ---- @user ---- shows how long the user has been in the room
- !kick ---- (X) ---- kicks user for X minutes, default is 0.25 minutes (15 seconds)
- !kill ---- ----- shut down the bot
- !lockguard ---- ---- toggle the lockguard
- !lockskip ---- (reason) ---- skip the song and move the dj back up (the position can be set with !lockskippos)
- !lockskippos ---- X ---- set the position to which lockskip moves the dj
- !motd ---- (X)/(message) ---- when no argument is specified, returns the Message of the Day, when X is specified, the MotD is given every X songs, when "message" is given, it sets the MotD to message
- !mute ---- @user ---- mute user
- !reload ---- ---- reload the bot
- !restricteta ---- ---- toggles the restriction on eta: grey users can use it once an hour
- !sessionstats ---- ---- display stats for the current session
- !skip ---- ---- skip the current song
- !status ---- ---- display the bot's status and some settings
- !timeguard ---- ---- toggle the timeguard
- !togglemotd ---- ---- toggle the motd
- !unban ---- @user ---- unban user
- !unmute ---- ---- unmute user
- !voteratio ---- @user ---- display the vote statistic for a user 

Resident DJ
-----------

- !link ---- ---- give a link to the current song



User
----

- !ba ---- ---- explains the Brand Ambassador rank
- !commands ---- ---- gives a link to the commands
- !cookie ---- (@user) ---- give a cookie to user
- !dclookup ---- ---- use dclookup on yourself
- !emoji ---- ---- a link to a list with emoji's
- !eta ---- ---- shows how long before you reach the booth
- !link ---- ---- when the user is the DJ, give a link to the current song
- !ping ---- ---- pong!


