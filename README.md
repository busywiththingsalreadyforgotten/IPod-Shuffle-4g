# IPod Shuffle 4g Scripts (modifed for windows 10)

Just a really quick hack of the [IPod-Shuffle-4g project](https://github.com/nims11/IPod-Shuffle-4g) to make it work on windows 10
(my apologies to the original coders!)

Just thought I'd post it here in case anyone else finds it useful

Additional Features Include:
* Automatic playlist creation (one playlist per artist)
* Optimisation of voiceover wav file creation (only creates voiceover wavs for new files)

#### Dependencies

This script requires:

* [Python 2.7](http://www.python.org/download/releases/2.7/)
* [Mutagen](https://code.google.com/p/mutagen/)
* [Balabolka](http://www.cross-plus-a.com/balabolka.htm) (for text to speech) 
** For german, requires download of microsoft voice "Microsoft Hedda Desktop"

I upload my tracks using musicbee and then have setup a hotkey to run the following command:
* python shuffle.py --create-playlists f: (where f: is the drive letter of my ipod shuffle)
