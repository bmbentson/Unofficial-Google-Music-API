An unofficial Python API for Google Music. The project is not supported or endorsed by Google.


###Features

* authentication
    * web client
    * music manager

* loading:
    * all song metadata
    * all user playlist titles and ids (not auto, yet)
    * songs from a specific playlist

* searching:
    * songs
    * artists
    * albums

* playlist:
    * creation
    * name changing
    * song addition and removal
    * deletion

* song:
    * downloading - gets a link and download count (GM allows 2 downloads per file)
    * metadata changing (to avoid surprises read protocol_info)
    * uploading - mp3 only as of now (unlike Google's music manager, it will upload multiple copies of the same file if tags differ. Google's backend will actively reject duplicate uploads, however.)
    * streaming - gets a url that works without authentication
    * removal from library

###Usage
gmapi.api.Api is the user-facing interface.
To get started, see example.py.

I'm currently working on better documentation. Experimental docs live [here](https://github.com/simon-weber/Unofficial-Google-Music-API/tree/master/docs/build/html/index.html) for now.

###Notes
This is a work in progress, so debug logging is enabled by default.
All logging is done to gmapi.log, and warnings and above are printed to	the console.
I don't	log anything authentication-related - you can check the  logs to be sure.



- - -
  
  
Feel free to contact me	with anything relating to the project. Bug reports, feature requests, and contributions are welcome.



Copyright (c) 2012 Simon Weber  
Licensed under the [GPLv3](http://www.gnu.org/licenses/gpl.txt).