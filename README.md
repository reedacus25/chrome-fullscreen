# chrome-fullscreen
Apple Script App to launch Chrome fullscreen

This is a really simple Apple Script I wrote to launch Chrome in fullscreen for a Mac Mini used for Google Meet in a conference room.

Download the scpt file, open in Script Editor.
Then File -> Export
Change the File Format to Application, then save.

I did run into some weirdness with MacOS permissions at first, and you will get some errors when trying to launch when it does the System Events call.

I think I had to reboot after giving it permission before it would actually run.

Then I added the application to login items (System Preferences -> Users & Groups -> $USER -> Login Items).
Now when the computer starts up, it launches a fullscreen instance of Chrome.
I then use an Elgato Streamdeck to control the Google Meet rooms using [this Chrome plugin](https://github.com/petele/StreamDeck-Meet).

I haven't worked too hard to figure out how to keep Chrome from periodically logging out the conference room user, but that is the only time keyboard and mouse are needed.

Hopefully this is useful to someone because it took a good bit of trial and effort to figure out this task that I expected to be pretty common and simple to accomplish.

I tested this on MacOS 11.5.1, 11.5.2, and 11.6.1.

When upgrading from 11.5.1 to 11.5.2 it appeared to break, causing me to need to recreate the app.
And again when upgrading to 11.6.1, I had the same thing happen, however a reboot seemed to cure it.
