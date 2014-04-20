basicBot
========

Usage
-----

Bookmark the following code. To run the bot, run the bookmark.

javascript:$.getScript('https://raw.githubusercontent.com/Yemasthui/basicBot/master/basicBot.js');

###Special settings###

Standard settings can be used. Both the default settings and an example of a custom settings file (uses the .json extension) are included.
To use a settings file, make a public url for it. An easy way to do this is to upload it to dropbox and get a public link to it.
Include the link (for example www.mysettings.com/settings.json ) like this in your room's description, followed by a space or an enter:

@basicBot=www.mysettings.com/settings.json


Credits
-------

I would like to thank the following people:

- Fungus: His Tastybot has been a source of inspiration for most of the features, and his help with coding problems has been invaluable to make this bot.
- TAT, Origin and other Litebot contributors: Their Litebot has inspired features like Roulette.
- Henchman: Never knew this undertaking would give me a friend too.


Copyright
---------

Copyright &copy; 2014
 
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


Bot features (all can be disabled or enabled through commands)
--------------------------------------------------------------

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

Commands:
---------

These can be found under the commands file.