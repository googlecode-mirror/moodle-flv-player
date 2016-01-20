Please note that many video hosting sites, such as YouTube, already have a generous cross domain policy file. If you want to display video from YouTube and similar video hosting services, it is not necessary to read this page.

## What is a crossdomain.xml policy file? ##

Cross domain policy files are a feature of Flash Player's security model. They give other domains permission for Flash files hosted on them to access content. When applications running on Flash Player in users' browsers from one domain, e.g. http://example.com/my_flash.swf, attempt to load content from another, e.g. http://anotherdomain.com/a_video.flv, Flash Player automatically attempts to load a file at the other domain's root, e.g. http://anotherdomain.com/crossdomain.xml. If the cross domain policy file fails to load for any reason or the file does not give permission to the domain where the Flash application is hosted, Flash Player throws a security error and doesn't load the requested content.

Here's an example of a crossdomain.xml policy file:

```
<?xml version="1.0" encoding="utf-8"?>
<cross-domain-policy>
<!-- Place top level domain name -->
<allow-access-from domain="www.example.com" secure="false"/>
<allow-access-from domain="www.example.com" to-ports="80,443"/>
<allow-http-request-headers-from domain="example.com" headers="*" />
<!-- use if you need access from subdomains. testing/www/staging.domain.com -->
<allow-access-from domain="*.example.com" secure="false" />
<allow-access-from domain="*.example.com" to-ports="80,443" />
<allow-http-request-headers-from domain="*.example.com" headers="*" />
</cross-domain-policy>
```

More details on how to configure cross domain policy files are available on Adobe.com's website: http://www.adobe.com/devnet/articles/crossdomain_policy_file_spec.html

## When do I need one? ##

You need a cross domain policy file when you want any Flash application hosted on your site to access content on another URL. For example, if your domain is http://example.com/ and you want to access content on http://anotherdomain.com/, then you need a cross domain policy file at http://anotherdomain.com/ that grants Flash applications hosted on http://example.com/ permission to do so. This is a security feature built into Flash Player itself and cannot be overridden.