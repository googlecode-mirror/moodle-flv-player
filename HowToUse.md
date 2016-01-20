# How to use the FLV Player #

  * Go to a Moodle course page
  * Select "Turn editing on"
  * Select "Add an activity" > "FLV Player"

The following form page will appear:

## General ##

<p><img src='http://matbury.com/tutorials/flv_name_description.png' alt='FLV Name and Description' width='800' height='425' /></p>

  * **Name** - This name appears as the text link on the Moodle course page
  * **Description** - Nuff said!


---


## Video Source ##

<p><img src='http://matbury.com/tutorials/flv_video_source.png' alt='FLV Video Source' width='802' height='169' /></p>

  * **Video URL** - Location of video file.
  * **Type** - Type of video. Sound, Image and Video automatically load files from Moodle course files directory. If set to YouTube, just copy and paste the YouTube.com page URL into VideoURL, e.g. http://www.youtube.com/watch?v=5lp1-OrycKs
  * **Streamer** - Gateway of streaming server. HTTP, Lighttpd and RTMP streaming are all possible depending on your site configuration. Please contact your site administrator about any streaming servers that are available.


---


## Appearance ##

<p><img src='http://matbury.com/tutorials/flv_appearance_notes.png' alt='FLV Notes' width='801' height='213' /></p>

  * **Notes** - Formatted text, images and other media are displayed under the video player.

<p><img src='http://matbury.com/tutorials/flv_appearance.png' alt='FLV Appearance' width='801' height='405' /></p>

  * **Width** - Width of video player
  * **Height** - Height of video player
  * **Skin** - Appearance of video player. There are currently 27 skins to choose from.
  * **Image** - Poster image that appears before learner clicks play. Not visible if Auto Start is set to true.
  * **Icons** -
  * **Logo** - Graphic logo that appears at top right of video player screen
  * **Control Bar** - Location of video player control bar
  * **Play List Position** - Location of play list (if XML play list file is provided instead of video file in Video URL.
  * **Play List Size** - Width of play list

The following are in hexidecimal values (white = FFFFFF, black = 000000, red = FF0000, green = 00FF00, blue = 0000FF, etc.):
  * **Back** - Control bar background color
  * **Front** - Control bar controls color
  * **Light** - Control bar volume and seek bar color
  * **Screen** - Video player background color


---


## Behaviour ##

<p><img src='http://matbury.com/tutorials/flv_behaviour.png' alt='FLV Behaviour' width='800' height='571' /></p>

  * **Auto Start** - If set to true, video starts playing immediately, if false, learner has to select play
  * **Full Screen** - Allow video player to expand to take over the entire screen (the same as YouTube.com)
  * **Stretching** - How the video stretches to fit the player dimensions
  * **Volume** - Volume of video audio
  * **Mute** - Mute video audio
  * **Repeat** - If XML play list is provided in Video URL, determines how list is played back
  * **Item** -
  * **Shuffle** - If XML play list is provided in Video URL, determines how list is played back
  * **Start** - Position at which video starts playing in seconds
  * **Buffer Length** - Allows a number of seconds of video to download before play back commences for smoother play back on slower connections
  * **Quality** - Quality of appearance of video in player (not the same as high/low definition!)
  * **Display Click** - What to do if the learner clicks on the video screen
  * **Link** - A link to a file or web page. Learners could download related materials in a ZIP file before or after watching
  * **Link Target** - How to navigate to the link (i.e. same page, new page, etc.)
  * **Resizing** -
  * **Plugins** - Currently only accessibility-1 is supported (see Timed Text Captions)
  * **Timed Text Captions** - An XML file containing video captions. Can be authored using the free MAGPie2 editor. Timed Text captions are part of the W3C SMIL specifications and similar to RealText captions.


---


## Metadata ##

<p><img src='http://matbury.com/tutorials/flv_metadata.png' alt='FLV Metadata' width='800' height='202' /></p>

  * **Author**
  * **Date**
  * **Title**
  * **FLV Description**
  * **Tags**


---


## Advanced ##

<p><img src='http://matbury.com/tutorials/flv_advanced.png' alt='FLV Advanced' width='801' height='254' /></p>

  * **Config XML File** - An XML file which contains all the JW FLV Player settings on this form page. Useful for saving time and easily changing the appearance of all FLV Players at once by editing the same XML file.
  * **JW Player Version** - Change this if you upgrade the JW FLV Player.
  * **Flash Player Version** - The minimum Flash Player version. If learner's version is lower, it triggers an automatic upgrade from Adobe.com. Learner must have administrator priveledges to perform an upgrade.
  * **Client** - A facility for developer debugging
  * **Trace Call** - A facility for developer debugging
  * **ID** - The required ID for the Flash Player on the FLV Player page. For Linux Operating Systems only.


---


## Commercial Licence Required ##

<p><img src='http://matbury.com/tutorials/flv_licence.png' alt='FLV Licence' width='801' height='173' /></p>

  * **About Text**
  * **About Link**

**Please note:** Do not change these settings without first purchasing a commercial licence from [Longtail Video](http://longtailvideo.com). Commercial licences are also required if your website hosts advertising or is otherwise considered commercial. Check with Longtail Video for further details. Cost of a single site lifetime commercial licence as of March 2009 was €30.

---
