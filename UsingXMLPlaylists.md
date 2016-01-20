# Using XML Playlists #

The JW FLV Player also supports playlists. A playlist is an XML file containing a list of videos to play which appear as a menu in the FLV Player window, like this:

<img src='http://matbury.com/tutorials/flv_playlist.png' alt='Playlist' width='554' height='252' />

---


## How to deploy a SMIL XML Playlist ##

<p><img src='http://matbury.com/tutorials/flv_video_source.png' alt='FLV Video Source' width='810' height='175' /></p>

  * In Video URL, select "Choose or upload a file"
  * Select or upload the desired SMIL XML playlist file
  * Select "XML Playlist" from the Type list

---


## How to show the playlist menu ##

<p><img src='http://matbury.com/tutorials/flv_playlist_params.png' alt='FLV Video Playlist Parameters' width='333' height='86' /></p>

The playlist menu is the list of videos that appears next to the FLV Player window. You can set the position and width of the playlist. In the Appearance section, do the following:

  * In Play List (position), select the desired position bottom, right, over or none
  * In Play List Size (pixels), set the desired width, e.g. 180

The JW FLV Player supports a number of other playlist formats. See the [JW Player documentation](http://developer.longtailvideo.com/trac/wiki/FlashFormats) for more details.

---


## Example SMIL XML Playlist ##

Filename: playlist.xml

```
<?xml version="1.0" encoding="utf-8"?>
<smil>
	<head>
		<meta name="title" content="Example SMIL playlist for the JW Player"/>
	</head>
	<body>
		<seq>
			<par>
				<video title="First FLV video" src="http://yourmoodleroot.com/file.php/99/yourvideo_1.flv" author="The video author" alt="This is an example of one video in an FLV playlist"/>
				<anchor href="http://www.thevideoauthor.org/"/>
			</par>
			<par>
				<video title="Second FLV video" src="http://yourmoodleroot.com/file.php/99/yourvideo_2.flv" author="The video author" alt="This is an example of the next video in an FLV playlist"/>
				<anchor href="http://www.thevideoauthor.org/"/>
			</par>
			<par>
				<video title="Third FLV video" src="http://yourmoodleroot.com/file.php/99/yourvideo_3.flv" author="The video author" alt="This is an example of the third video in an FLV playlist"/>
				<anchor href="http://www.thevideoauthor.org/"/>
			</par>
			<par>
				<video title="Youtube video with start" src="http://youtube.com/watch?v=IBTE-RoMsvw" author="the Peach Open Movie Project" alt="Big Buck Bunny is a short animated film by the Blender Institute, part of the Blender Foundation." begin="10"/>
				<anchor href="http://www.bigbuckbunny.org/"/>
			</par>
		</seq>
	</body>
</smil>
```

**Please note:** It is necessary to use absolute paths to the FLV video files, i.e. `http://yourmoodleroot.com/file.php/99/file.flv`

There's a list of SMIL XML authoring tools here: http://www.w3.org/AudioVideo/#Authoring


---


## XML Playlist Formats ##

The JW FLV Player supports several different XML playlist formats:

  * ASX
  * ATOM
  * RSS
  * XSPF

Please consult this page for more details: http://developer.longtailvideo.com/trac/wiki/Player5Formats This page links to some examples but you may have to view page source in your browser to see the actual XML code.


---


## SMIL XML authoring tools ##

[Please see this page for useful links about SMIL XML and authoring tools.](http://code.google.com/p/moodle-flv-player/wiki/TimedTextCaptioning)