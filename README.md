# tizlast
Scrobble to last.fm when using Spotify via command line.

If you use [Tizonia](http://tizonia.org/) to listen to music on Spotify but also want to keep track of your listening history with last.fm, this might help you out. 

### Prerequisites
+ python
+ tizonia installed to your PATH
+ spotify login information in Tizonia .config file (optional, see Troubleshooting)
+ last.fm API account. You can register for one [here](https://www.last.fm/api/account/create).
+ pylast ```pip install pylast```

### Usage
Edit the script to include your last.fm and API info, and add tizlast to your PATH. Then,

```tizlast [album name] [artist name (optional)]```

### Modifications
You can easily change this to work with other streaming platforms, just change the Tizonia call accordingly. You can also change this to work for individual tracks rather than albums, but you'll have to change the scrobbling function as well. I don't know how to get this to work easily for playlists.

### Troubleshooting
If it doesn't work, it's most likely because the Spotify login via config file isn't working. If you're not sussed out by passing login information through the command line, uncomment line 24, add your Spotify login info, then comment out line 23.
