# Better Time (Sans Fight)
This project is a fork of [Bad Time Simulator](https://jcw87.github.io/c2-sans-fight/), which is itself a clone of the sans fight from [Undertale](http://undertale.com/).
It was made with [Construct 2](https://www.scirra.com/construct2).

NOW AVAILABLE! [Custom attacks guide](Documentation/README.MD)
-----------------------------------------------------

Changes
-------
- The game will prompt you to enter a name in the same style as Undertale at the start.
- There is a settings menu that lets you control music volume, sound volume, and LOVE (which affects your max HP).
- You can now hold escape during the battle to quit to the main menu.

Technical Changes
-----------------
- The "Sound" function can now take a third parameter for the sound tag. If a sound tag is provided, it will stop the sound associated with that tag before playing the new sound.
- All calls to the Audio plugin to start playing a sound have been replaced with calls to the "Sound" and "Music" functions.
- The "Sound" and "Music" functions have been moved to a new event sheet named "Common", which also controls initialization like loading stuff from LocalStorage. This event sheet is included in most event sheets.
- The HP text and the KR sprite now automatically position themselves to the right of the HP bar so that a lower LOVE value doesn't screw up the display.
- Added a new VPad control "Quit" (and a touch button for activating it), exiting custom attacks now uses this control instead of the "Cancel" control.
- Main menu now has unbounded scrolling, but locks the scroll Y to what would normally be the layout's top border.
- RPGText now has a speed component.
- The NameScreen layout now exists. [Hopefully this is temporary](https://www.reddit.com/media?url=https%3A%2F%2Fpreview.redd.it%2Fuy7idfysnhe31.png%3Fauto%3Dwebp%26s%3D71c6984b58be360b001a5961a3522087870ad4ea) and gets replaced by a proper menu on the MainMenu layout.

Known Issues
------------
- Heart hitbox is probably not accurate.
- On the sans_platforms4 and sans_platforms4hard attacks, the platform is supposed to accelerate from 0 to its full speed, but I was lazy and started it at full speed immediately. This is only a problem if you try to dodge the bones without jumping.
- Sans dialog is missing. I may add something at some future date, but I have no intention of putting the original text in, as it really only makes sense in the context of the whole game.

Contact
-------
If you want to contact jcw87 for some reason, you can do so through the following:

- ~~[Facepunch](https://facepunch.com/member.php?u=13155)~~ R.I.P. Facepunch
- [Steam](http://steamcommunity.com/id/Jcw87/)