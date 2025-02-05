=== Inlinefeed ===
Contributors: dkruyt
Donate link: http://kruyt.org
Tags: rss, atom, feed, inline, embed, rdf
Requires at least: 2.5
Tested up to: 2.5.1
Stable tag: 2.01

With the inlinefeed plugin you can display and embed RSS/ATOM feeds in your Wordpress posts and pages.

== Description ==

With the inlinefeed plugin you can display and embed RSS/ATOM feeds in your Wordpress posts and pages using the following shortcode:

`[inlinefeed rss_feed_url="http://feed.xml"]`

NOTE: From version 2.0 you can only use the shortcode [inlinefeed], the old style `<!--rss:[URL]-->` doesn't work anymore! If you upgrade
from a 1.xx version, then you must change from `<!--rss:[URL]-->` to `[inlinefeed rss_feed_url="[URL]"]` style.

FILTER USAGE

* Simple:
   
Just put a `[inlinefeed rss_feed_url="http://yourfeed.rdf"]` in your post, and the feed will show up.

Left as rss for backwards compatibility but will work with ATOM feeds as well.

* NAMED PARAMETERS

For some customisation there are some options you can use.

- display (1-100): Show the number of lines from the feed.
- rss_feed_url (url): The RSS/ATOM URL.
- displaydescriptions (true/false): Show the discription / content of the feed, default true.
- truncatetitle (false/1-100): Truncate long title headers after x caracters. Or false if no truncate (default).
- newwindow (true/false): Open links in new window?
- displayfeedname (true/false): Display the name of the feed, default true.

Examples:

`[inlinefeed rss_feed_url="http://www.osnews.com/files/recent.rdf" displaydescriptions=true truncatetitle=false newwindow=true display=15]`

`[inlinefeed rss_feed_url="http://kerneltrap.org/rss.xml" displaydescriptions=true truncatetitle=false newwindow=false]`

`[inlinefeed rss_feed_url="http://slashdot.org/index.rss" displaydescriptions=true truncatetitle=20]`

`[inlinefeed rss_feed_url="http://www.securityfocus.com/rss/news.xml" displayfeedname=false displaydescriptions=true truncatetitle=false]`

`[inlinefeed rss_feed_url="http://www.ipodhacks.com/ipodhacks.xml" displaydescriptions=true truncatetitle=false]`

`[inlinefeed rss_feed_url="http://www.viruslist.com/en/rss/virusalerts" displaydescriptions=false truncatetitle=false display=5]`

`[inlinefeed rss_feed_url="http://tweakers.net/feeds/mixed.xml"]`

Finally note the whole thing must be on ONE line.  No line breaks or else it won't work.

If you want to use a gziped rssfeed try you must add gzip support to wordpress, take a look here: http://wordpress.org/extend/plugins/class-snoopyphp-gzip-support/

Live examples:

http://kruyt.org/wordpress/inlinefeeds/security

http://kruyt.org/wordpress/inlinefeeds/news

* ChangeLog

2.01 truncate title accpets now a nummeric value. New option, displayfeedname.
2.00 Now uses the wp 2.5 shortcode.
1.62 Error handling and headers are giving descriptions and are clickable.
1.6 Added option newwindow. If you want to open in a new window.
1.5 Fixed a bug that the feed got bumped up to the top of the page.
1.4 XHTML compliant.
1.3 Truncate title.
1.2 minor fixes.
1.1 Initial release.

== Installation ==

Just unzip in your plugin folder, and actived in your wordpress admin panel.
