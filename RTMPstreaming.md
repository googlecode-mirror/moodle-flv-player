## How to deploy RTMP streaming with the FLV Player module. ##

This page describes how to modify the FLV Player module to support RTMP streaming servers. It is not recommended for beginners as it requires some knowledge of PHP code.

  * Open the file at: MOODLE/mod/flv/lib.php
  * Find the following lines (at around 545 - 552):

```
function flv_list_streamer() {
	global $CFG;
	return array('' => 'none'
			//, $CFG->wwwroot.'/mod/flv/xmoov/xmoov.php' => 'Xmoov-php (http)'
			//, '' => 'Lighttpd'
			//, 'rtmp://yourstreamingserver.com/yourmediadirectory' => 'RTMP'
	);
}
```

  * Un-comment the line: , 'rtmp://yourstreamingserver.com/yourmediadirectory' => 'RTMP'
  * Change it to reflect to location of your streaming server
  * It's also a good idea to change the 'RTMP' to something like 'My RTMP Streaming Server', 'Acme Streaming Server'.

Your modified code should look something like this, assuming that you're using an RTMP streaming service by "Acme":

```
function flv_list_streamer() {
	global $CFG;
	return array('' => 'none'
			, 'rtmp://acmestreaming.com/video' => 'Acme Streaming Server'
	);
}
```

The FLV Player Module can support any number of RTMP streaming servers. For example:

```
function flv_list_streamer() {
	global $CFG;
	return array('' => 'none'
			, 'rtmp://acmestreaming.com/video' => 'Acme Streaming Server'
			, 'rtmp://flashmediaserver.com/media' => 'FMS'
			, 'rtmp://wowza.com/flics' => 'Wowza'
	);
}
```


**Please note:**

  1. Video file names shouldn't include the .flv file extension, i.e. "myvideo" not "myvideo.flv"
  1. There must be a crossdomain.xml policy file configured to allow your Moodle site's domain name at the root of the RTMP server public directory, i.e. rtmp://acmestreamingserver.com/crossdomain.xml For more details, please see: http://kb2.adobe.com/cps/142/tn_14213.html