<img src='http://matbury.com/tutorials/screenshot_flv_player_with_subtitles.jpg' alt='FLV Player with TimedText captions' width='600' height='317' />

The FLV Player Module makes it easy to deploy TimedText captions with your video. TimedText is a W3C web standard for video and audio captioning. You can see an example of TimedText captioning with the FLV Player module on my [Moodle](http://matbury.com/moodle/course/view.php?id=9). Selecting "Login as guest". A user account is not necessary.


**TimedText caption XML data format:**

```
<tt xmlns="http://www.w3.org/2006/10/ttaf1">
 <body>
  <div xml:id="captions">
   <p begin="00:00" end="00:08">matbury.com</p>
   <p begin="00:08" end="00:09.9">Thank you. Thank you very much ladies and gentlemen.</p>
   <p begin="00:10" end="00:14.9">Um, we'd like to do a sketch for you now. It's called the Hedge Sketch...</p>
   <p begin="00:14" end="00:22">...and it's set in a shop. The Hedge Sketch. Thank you very much indeed.</p>
   <p begin="00:22" end="00:24">Hello, I'd like to buy a hedge please.</p>
   <p begin="00:24" end="00:26">Good morning sir, how can I help you?</p>
   <p begin="00:26" end="00:28">Well, what sorts have you got?</p>
  </div>
 </body>
</tt>
```

You can write TimedText caption files with any text editor manually (Windows Notepad is not recommended) or there are free software packages that make creating TimedText much easier. Here's a brief outline of what the TimedText caption code represents:

**begin** The time that the caption appears - "**minutes:seconds.0**"

**end** The time that the caption disappears - "**minutes:seconds.0**"


If the begin time of the next caption overlaps, it will replace the current caption. In other words, if you want captions to appear in sequence without any gaps, the end parameters are not necessary. e.g.:

```
<tt xmlns="http://www.w3.org/2006/10/ttaf1">
 <body>
  <div xml:id="captions">
   <p begin="00:00" >matbury.com</p>
   <p begin="00:08" >Thank you. Thank you very much ladies and gentlemen.</p>
   <p begin="00:10" >Um, we'd like to do a sketch for you now. It's called the Hedge Sketch...</p>
   <p begin="00:14" >...and it's set in a shop. The Hedge Sketch. Thank you very much indeed.</p>
   <p begin="00:22" >Hello, I'd like to buy a hedge please.</p>
   <p begin="00:24" >Good morning sir, how can I help you?</p>
   <p begin="00:26" >Well, what sorts have you got?</p>
  </div>
 </body>
</tt>
```


To deploy a TimedText caption XML file for a video with the FLV Player module, do the following:

  * On the desired Moodle course page, select "Turn editing on"
  * Select "Add an activity..." > "FLV Player"
  * On the FLV Player form, if necessary, select "Show advanced"
  * Select or upload the desired video and complete the desired parameters
  * At the bottom of the "Behaviour" panel type "accessibility-1" in the "Plugins" text area
  * In "TimedText Captions" select "Choose or upload a file..."
  * Choose or upload the desired TimedText captions file
  * Select "Save changes"
  * Review the captions

## Useful links ##

  * [Wikipedia.org Timed Text](http://en.wikipedia.org/wiki/Timed_Text)

  * [W3C Timed Text - Why a Standardized Timed-text Format?](http://www.w3.org/AudioVideo/timetext.html)

  * [W3C Timed Text Working Group](http://www.w3.org/AudioVideo/TT/)

  * [W3C Timed Text - List of authoring tools](http://www.w3.org/AudioVideo/#Authoring)