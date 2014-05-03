NGINX FancyIndex Theme
===

A prettier theme for nginx' fancyindex module. Further details about this excellent
module can be found at the dev's [github page](https://github.com/aperezdc/ngx-fancyindex).

#####Usage:
 - Compile nginx with the fancyindex module.
 - Include the contents of 'fancyindex.conf' in your location directive of your nginx conf.
 - copy the remaining items in your web root under 'fancyindex'.
  - header.html
  - footer.html
  - css\fancyindex.css
  - fonts\\*
  - images\breadcrumb.png
 - Restart your nginx server.

#####Added/Modified:
 - Mime type icons from [Splitbrain](http://www.splitbrain.org/projects/file_icons)
  - Icons default to enabled on large devices and off on small devices like phones.
  - If you'd prefer no icons at all: copy css\fancyindex_NoIcons.css css\fancyindex.css
 - Slightly better handling of mobile CSS click areas.

![Image1](https://raw.githubusercontent.com/TheInsomniac/Nginx-Fancyindex-Theme/master/images/fancyindex.png)