
Auto-Anime-Downloader---XDCC
============================




Automated anime downloader using irc xdcc instead of torrents :)

THIS IS LINUX ONLY FOR NOW!!! THIS IS OLD AND MIGHT NOT WORK ANYMORE.
FOR WINDOWS, USE THIS:
[WeebIRC](https://github.com/RareAMV/WeebIRC)
This little irc client comes with a build in nibl.co.uk search function with the ability to batch download anime by selecting the search results :D.

Yep, I made this mainly for the raspberry pi.
So, before this works you will have to set things up correctly:

1. sudo apt-get install mono-complete.

2. sudo apt-get install irssi.

3. run irssi by typing in terminal: irssi.

4. close it by typing /quit.

5. open /home/(user) and make sure that you can see hidden folders.

6. locate .irssi folder and open it.

7. put AutoAnimeDowloader.exe, config and settings.ini in it.

8. change nickname etc in config file to your liking, do not use the one provided with it, since it might be in use.

9. open AAD SetupGUI and follow the steps shown to you when launched (download the .exe only if you do not want to edit/change the code).

10. start AutoAnimeDownloader.exe by typing cd /home/(user)/.irssi, or if you are already in home: cd /.irssi 
and then mono AutoAnimeDownloader.exe

11. now it works, your files will be dlld to you home/(user) folder, option to change this will be added in the future

12. to run it 24/7, you will have to lauch it from the raspberry pi itself, if you use ssh it will
stop the script when you close the ssh connection.

YOUR DONE!

____________________________________________________________________________________________________
Search examples:
-------------------

Search Examples: 

Horriblesubs 720p <- downloads all new 720p episodes from horriblesubs

Horriblesubs Psycho-Pass 2 720p, Horriblesubs Shirobako 1080p <-downloads all new psycho pass 2 eps in 720p, 
and all new shirobako 1080p episodes.

____________________________________________________________________________________________________

Future functions:
-------------------
Delete anime subscription

Windows functionality

Batch download function

Use custom rss feed

Change Download Location 

In the far, far away future mal implementation, since its logically that once downloaded you watch it.

Auto remove function(like delete in 30 days)(only if requested);

____________________________________________________________________________________________________
How it works:
------------------
Scans first item on nyaas rss, search on intel.haruhichan.com on the bot page for a pack containing the 
anime name from the rss feed, open irssi and let it automaticly join #intel and automaticly run command 
/msg [bot] xdcc send #packnumber and it starts downloading.

____________________________________________________________________________________________________
Versions:
------------------

--- 0.1 released (first version count)

added multiple anime subscription support

possible fix for crash when anime is not yet uploaded on intel.haruhichan

known problems:

While I tested it, it crashed again because of the fix above, atleast that is what I think, it was at night and i forgot to save the ssh log.

--- 0.1.1 released 
functional gui added

able to download animes from different sub groups(per anime)

able to change bot you want to download from(per anime)

almost functional on windows, almost....

known problems: both gui and autoanimedownloader are not able to create there log and other files they write to. They will 
crash if they are not present, you can find the files in the needed files directory, they can also help as an example if
you want to use a text editor to edit the settings.ini for example.
____________________________________________________________________________________________________
Future Vision:
------------------
A popcorn time ish anime watcher / downloader. And it will be more reliable since it does not need the use of torrents, xdcc are generaly faster then torrents, and nomatter how old the file on the server is, it will have equal speeds to new one(but it has to be on the server). No more waiting until it is seeded, it will be press and play :). Now, this might never become true, since that requires a shit ton of work and I am on my own, with an programming language wich i just started at, and my study just starting, which requires a lot of time. So for now it will be a simple automated downloader :)
