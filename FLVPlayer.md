A duplicate copy of this page can be found in [Moodle documentation](http://docs.moodle.org/en/FLV_Player).

## Summary ##

The JW FLV Player 4.3 is a powerful and extremely versatile application for viewing video on web pages. The FLV Player Activity Module acts as a wizard to deploy and configure the JW FLV Player. It doesn't require any coding abilities and is possibly the quickest, easiest, most comprehensive and robust method of deploying and configuring video in Moodle.

<img src='http://matbury.com/wiki/images/flv_player.jpg' alt='FLV Player' width='500' height='279' />

Jeroen Wijering's FLV Player is an ideal method to deploy Flash video in Moodle. It's extremely versatile and supports a number of features that are particularly useful for e-learning:

  * [Section 508](http://en.wikipedia.org/wiki/Section_508) (accessibility) compliance.
  * Support for [TimedText XML](http://en.wikipedia.org/wiki/Timed_text) and  RealText (SMIL) captioning.
    * A selection of plugins and skins are available.
  * Developers can create their own skins and plugins.

---


## Licence ##

Although this Moodle module is open source, '''Jeroen Wijering's FLV player, included within, is not open source'''. It is commercial software which is available free for noncommercial use, but requires a (small) licence payment for all other use. Please see [Jeroen Wijering's web site](http://www.longtailvideo.com/) for licensing details.

'''Here's a quote from Longtailvideo.com''':

''Why Buy a License? If you don’t buy a commercial license, you cannot use a JW Player on (i) a site that has ads; (ii) a corporate site; or a (iii) CMS. Our licenses are very inexpensive, so what are you waiting for? Buy a license today.''

The price for a lifetime licence for a single domain on 7th February 2009 was €30. [Check here for questions about whether or not you need a licence and what type](http://www.longtailvideo.com/support/forum/Licensing-Questions/).

---


## Supported Video Formats ##

Supports all video formats supported by Flash Player 9 and above. Currently (5th February 2009) file types:

  * FLV
  * MP4
  * MP4V
  * M4V
  * M4A
  * 3GP
  * 3G2
  * MOV


It also supports the new standard high-definition CODEC, H.264, and AAC audio (Advanced Audio Compression) which is similar to MP3 but gives better quality at very low bit-rates.

---


## Captioning ##

The FLV Player module makes it much easier to deploy captions with the JW FLV Player. Simply do the following:

  * Prepare the video and TimedText (RealText is also supported) files.
  * Upload them to the moodledata course directory (you can also upload these from the FLV Player module form)
  * Create an instance of the FLV Player module and select the video file and desired parameters.
  * Select Show Advanced if not already shown.
  * At the bottom of the Behaviour section, type accessibility-1 into the Plugins text input area.
  * Select Choose or upload file in the Timed Text Captions input area and select or upload and select the desired TimedText captions file.
  * Select Save changes (Moodle 1.8) or Save changes and preview (Moodle 1.9)


Here are example [FLV video and TimedText caption XML](http://matbury.com/assets/captions_example.zip) to download and try (7.75 MB).

[MAGpie2 captioning editor](http://ncam.wgbh.org/webaccess/magpie/magpie_help/introduction.html) can export Adobe Flash WC3 DFXP captioning files which are compatible with JW FLV Player accessibility-1 plugin. However, the editor cannot play FLV files therefore an intermediary video file type, such as AVI, is necessary for creating caption files, i.e. create and export the caption file before encoding the video to FLV.

---


## Playing YouTube.com Videos ##

Playing videos directly from YouTube.com's servers is possibly the easiest way to play videos with the FLV Player Activity Module. Just follow these steps:

  * Find the video you want to show on YouTube.com
  * On a Moodle course page, select 'FLV Player' from the 'Add an activity...' list
  * On the YouTube.com video page, copy the URL in your browser's address bar, e.g. http://www.youtube.com/watch?v=5lp1-OrycKs
  * Now paste the URL in the 'Video URL' text field of the FLV Player form
  * Select 'Show Advanced' if not already set
  * Select 'youtube' from the 'Type' list
  * Select 'Save Changes' (Moodle 1.8) or 'Save and Preview' (Moodle 1.9) at the bottom of the FLV Player form
  * The YouTube.com video should play and all the parameters, such as icons, links, etc. will still function.

---


## Streaming ##

There are two main types of video connection, '''progressive download''', where the video FLV file is downloaded into the browser cache and the user can start to view the video content after a second or two, and '''streaming''', where specific portions of the video stream are served to the video player as and when requested. Progressive download is the easiest to implement and the most commonly used.

The JW FLV Player supports:

  * Progressive download (default)
  * [HTTP streaming](http://www.longtailvideo.com/support/tutorials/HTTP-Video-Streaming) (pseudo-streaming)
  * [LIGHTTP](http://www.lighttpd.net/) streaming
  * [RTMP](http://en.wikipedia.org/wiki/Real_Time_Messaging_Protocol) streaming ([Red5](http://www.osflash.org/red5) and [Flash Media Server](http://en.wikipedia.org/wiki/Flash_Media_Server))

---


## Notes ##

Allows course content developers or teachers to include notes under the video player. Includes text formatting and embedded images and other media. Ideal for lecture notes, key information, summaries and explanations, etc.

---


## Skins ##

Skins are a quick and easy way to change the appearance of JW FLV Player. The FLV Player Activity Module comes supplied with 27 skins which you can select from a list.

  * [JW FLV Player skins](http://www.longtailvideo.com/addons/skins).

---


## Plugins ##

Plugins add extra functionality to JW FLV Player. They are hosted on LongTail video's website so no downloading or installing is necessary. Simply type the name of one or more of the plugins you require in the Plugins text input area in the Behaviour section of the FLV Player Activity Module form.

The FLV Player module only explicitly supports the accessibility-1 plugin which displays TimeText captions (part of the W3C SMIL specification). The other plugins are mostly related to social networking sites, web analytics and other features. Support for more plugins may be added if the demand is high.

Available plugins are:

  * accessibility-1 - Displays TimedText captions (supported by FLV Player module)
  * viral-1
  * rateit-1
  * drelated-1
  * embed-1 - Allows learner to copy and paste embed code for video
  * tipjar-1 - Allows donations
  * googlytics-1
  * revolt-1
  * yourlytics-1
  * yousearch-1 - Allows learner to search YouTube.com
  * searchtoob-1 - Same as above
  * quickkeys-1 - Allows learner to control video player with the keyboard
  * metaviewer-1 - Displays video file metadata
  * hd-1 - Allows learner to switch to a high definition version of the video
  * soundproxy-1
  * clickproxy-1


There are also subscription and paid for plugin services available. [Find documentation and further details here.](http://www.longtailvideo.com/addons/plugins)

---


## Module Form ##

The module form allows users to set most of the parameters supported by JW FLV Player 4.3. [You can find documentation on the following parameters here.](http://developer.longtailvideo.com/trac/wiki/FlashVars)

### Source ###

  * **flvfile** 'Video URL'
  * **type** 'Type'
  * **streamer** 'Streamer'

### Appearance ###

  * **width** 'Width'
  * **height** 'Height'
  * **skin** 'Skin'
  * **image** 'Image'
  * **icons** 'Icons'
  * **logo** 'Logo'
  * **controlbar** 'Control Bar'
  * **playlist** 'Play List (position)'
  * **playlistsize** 'Play List Size (pixels)'
  * **backcolor** 'Back Color'
  * **frontcolor** 'Front Color'
  * **lightcolor** 'Light Color'
  * **screencolor** 'Screen Color'


### Behaviour ###
  * **autostart** 'Auto Start'
  * **fullscreen** 'Full Screen'
  * **volume** 'Volume'
  * **mute** 'Mute'
  * **flvstart** 'Start (position in seconds)'
  * **duration** 'Duration (seconds)'
  * **flvrepeat** 'Repeat'
  * **shuffle** 'Shuffle'
  * **bufferlength** 'Buffer Length (seconds)'
  * **quality** 'Quality'
  * **displayclick** 'Display Click'
  * **link** 'Link'
  * **linktarget** 'Link Target'
  * **item** 'Item'
  * **resizing** 'Resizing'
  * **stretching** 'Stretching'
  * **plugins** 'Plugins'
  * **captions** 'Timed Text Captions'


### Metadata ###

  * **author** 'Author'
  * **flvdate** 'Date'
  * **title** 'Title'
  * **description** 'FLV Description'
  * **tags** 'Tags'


### Advanced ###

  * **configxml** 'Config XML File'
  * **version** 'JW Player Version'
  * **client** 'Client'
  * **tracecall** 'Trace Call (debugging)'
  * **flvid** 'ID (For Linux OS Users Only)'
  * **abouttext** 'About Text'
  * **aboutlink** 'About Link'

---


## Issues ##

If you have any problems or issues with the FLV Player module, please list them, as clearly as you can, here.


## Resolved Issues ##

  * Browsers cached video files, images, icons and XML files. Users still saw old (cached files) after they had been updated on the server. The FLV Player Activity Module now prevents caching.

---


## See Also ##

  * [NCAM MAGpie2](http://ncam.wgbh.org/webaccess/magpie/) (Media Access Generator) for authoring caption and subtitle files
  * [Jeroen Wijering's web site](http://www.longtailvideo.com/) Including plugins, skins, tutorials and licensing details.
  * An article on the [Closed Captioning](http://www.digital-web.com/articles/captions_flash_video/) component in Flash CS3 and its benefits for accessibility.
  * [Matt Bury's website](http://matbury.com/) FLV Activity Module project developer.
  * [Xmoov](http://xmoov.com/xmoov-php/) HTTP (pseudo) streaming open source project.
  * [RTMP](http://en.wikipedia.org/wiki/Real_Time_Messaging_Protocol) streaming media servers
  * [Red5](http://www.osflash.org/red5) open source media server
  * [Adobe Flash Media Server](http://www.adobe.com/products/flashmediaserver/)
  * [Lighttp](http://www.lighttpd.net/) open source project which includes a streaming server


**Please note:** MAGpie2 can export TimedText caption files for JW FLV Player but its video player does not support the FLV file type. It is therefore necessary to use an intermediary video file type, such as AVI, in order to create the captions.

---


### Other Projects by Matt Bury ###

  * SWF Activity Module, in development, which will enable deployment of Flash and Flex Framework learning applications (RIAs) in Moodle and leverage AMFPHP (Flash Remoting).