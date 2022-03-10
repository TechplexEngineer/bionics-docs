---
title: Archiving Match Footage
description: How to save match footage from twitch streams
# weight: 40
---

1. Download the videos from twitch

	1. Create a file containing a list of URLs to be downloaded eg. [videos.txt](videos.txt)
	2. Use `youtube-dl` or a more modern fork like `yt-dlp` to download each video 
	{{< highlight bash>}}youtube-dl -a videos.txt -f 1080p --external-downloader axel{{</highlight>}}

2. Join the downloaded files
	
	1. Create a list of files to be joined eg. [list.txt](list.txt)
	{{< highlight bash>}}find . -iname "*.mp4" -exec sh -c $'a="$1"; echo "file \'$a\'" >> list.txt' shell {} \;{{</highlight>}}
	2. Use FFMPEG to join the files specified by list.txt 
	{{< highlight bash>}}ffmpeg -f concat -safe 0 -i list.txt -c copy output.mp4{{</highlight>}}

3. Use FRC Video Splitter to spit matches
4. Upload to youtube 