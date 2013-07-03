jPlayer-for-httpd
=================

Use jPlayer to listen to songs in Apace httpd directory listings

This is a small patch to inject jPlayer in to httpd directory listings of mp3s. ¬
Put the .htaccess file in a directory that applies to all the directories of mp3s you want to listen to.¬
The .htaccess file injects player.html in to the HTML generated for each directory listing. The player.html¬
file loads the javascript and css assets of jPlayer, then finds all anchors on the page that point to mp3s.¬
The script in player.html then creates a jPlayer playlist of all the mp3s and hides the original directory listing.¬
¬
Things you need to do:¬
1. Put .htaccess in a directory that applies to your mp3 directories¬
2. Update the ReadmeName path in .htaccess to point to player.html
3. Update the paths to CSS and JS assets in player.html to use absolute URLs to the jplayer scripts and stylesheets.¬

References
==========
- [jPlayer](https://github.com/happyworm/jPlayer)
- [.htaccess guide](http://perishablepress.com/better-default-directory-views-with-htaccess/)
