This page describes some of the "ins and outs" of uploading video to a Moodle installation for deployment by the FLV Player.


---


## What's maximum upload file size? ##

If you want to use the Moodle file manager tool, in most cases you'll have to increase the maximum upload file size setting. This is not set by Moodle or the FLV Player module, it's a server setting. Administrators have the option to reduce the maximum upload file size on an entire Moodle installation or on a course by course basis.

On hosted servers, the default maximum is usually 2Mb which is equivalent to about 2 minutes of highly compressed video.

Changing the maximum upload file size varies depending on your server hosting and many other things. For more information, follow this link to a variety of Moodle forum posts (user or guest user login is required): http://moodle.org/mod/forum/search.php?search=change+max+upload+file&id=5


---


## I'm using FTP to upload my video files. Where should I put them? ##

If you upload a media file using the Moodle file manager tool, it is stored in the current course's media directory in the `/moodledata/` directory.

<img src='http://matbury.com/tutorials/swf_moodledata.gif' alt='moodledata directory' width='136' height='291' />

The numbered directories nested inside `/moodledata/` are directories that contain files uploaded for a particular course. You can find out which numbered directory the files for a course are stored in by going to the course page and looking in the browser address bar. You should see something like this:

`http://MOODLE/course/view.php?id=1`

The number after `?id=` is the number of the course directory. So the course files for the course page above are in `/moodledata/1/...`

Likewise, if you upload files using the Moodle course files manager, they will be stored in this directory.

Please note that a course directory is only created by Moodle when the first file has been uploaded.


---


## How does the FLV Player access `/moodledata/` course video files? ##

The FLV Player accesses files stored in a `/moodledata/` course directory by linking to them using absolute paths, like this:

`http://MOODLE/file.php/1/photos/example_photo_1.jpg`

`http://MOODLE/file.php/1/photos/example_photo_2.jpg`

`http://MOODLE/file.php/1/audio/example_audio_1.mp3`

`http://MOODLE/file.php/1/audio/example_audio_2.mp3`

etc.

The `MOODLE/file.php` script automatically manages access and permissions so that only users logged in on course can access files stored in the corresponding `/moodledata/` course directory. Also, search engines cannot index files stored in `/moodledata/`.

The recommended location for all media files for a course is in the corresponding moodledata course directory. The moodledata directory is situated outside the public HTTP directory and so can only be accessed either by FTP or by using Moodle's file manager tool. Keeping media files in non-public directories prevents other websites from linking to your video files thereby using server resources that you are paying for, also known as "leeching".

If you would like to make your videos available to the general public, I recommend using a free video hosting service like YouTube.com which will make your videos exceptionally easy for people to find and will help to bring new users, via a link, to your Moodle installation, while costing you nothing but your time! :)