NGINX FancyIndex Theme
===

A prettier theme for nginx' fancyindex module. Further details about this excellent
module can be found at the dev's [github page](https://github.com/aperezdc/ngx-fancyindex).

####NOTE:
NGX-FANCYINDEX truncates the file name to 50 characters subtracts 3 and then
appends a "..>" to the truncated name. This can be fixed by recompiling
NGX-FANCYINDEX after changing line 55 of "ngx_http_fancyindex_module.c":

From:

    #define NGX_HTTP_FANCYINDEX_NAME_LEN 50

To:

    #define NGX_HTTP_FANCYINDEX_NAME_LEN 500 (or some other number greater than 50)

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
 - Added HTML5 History for quicker page transitions.
  - This can be disabled by commenting out the script tag in footer.html
 - Fixed CSS issues on older versions of FF

#####Addendums:
 - If you want your 'Parent Directory/' listing back in your file listings:
  - Read: [This Issue](https://github.com/TheInsomniac/Nginx-Fancyindex-Theme/issues/1#issuecomment-43936700)

![Image1](https://raw.githubusercontent.com/TheInsomniac/Nginx-Fancyindex-Theme/master/images/fancyindex.png)

![Image1](https://raw.githubusercontent.com/TheInsomniac/Nginx-Fancyindex-Theme/master/images/fancyindex1.png)

![Image1](https://raw.githubusercontent.com/TheInsomniac/Nginx-Fancyindex-Theme/master/images/fancyindex2.png)
