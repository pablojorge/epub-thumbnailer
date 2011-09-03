---
layout: default
title: epub-thumbnailer
---

[epub-thumbnailer](http://github.com/marianosimone/epub-thumbnailer) is a little script I wrote because I wanted to see thumbnails of my epub books while browsing my collection:

<div style="text-align:center" markdown="1">
    ![There are no thumbnails for epub files before using epub-thumbnailer](images/epub-thumbnailer-without.png)

Thumbnails for pdf, but not for epub
</div>

After doing some googling, and not being able to find what I wanted (but [learning](http://ubuntuforums.org/showthread.php?t=278162) [something](http://ubuntuforums.org/showthread.php?t=1046678) about the [matter](http://library.gnome.org/devel/integration-guide/stable/thumbnailer.html.en)), I came up with epub-thumbnailer (you'll find download and install instruction at [GitHub](http://github.com/marianosimone/epub-thumbnailer)):

<div style="text-align:center" markdown="1">
    ![epub-thumbnailer adds thumbnails to epub files](images/epub-thumbnailer-with.png)

thumbnails for everyone!
</div>

which is not only better than nothing, but also better than pfd thumbnails, as it displays the cover, and not just the first page.

epub-thumbnailer can be integrated with nautilus, but also used as a stand-alone script, or even a a tool for some other project, you just have to invoke:

    {% highlight bash %}
    user@computer:$ epub-thumbnailer EPUB OUTPUT SIZE
    {% endhighlight %}

For example:

    {% highlight bash %}
    user@computer:$ epub-thumbnailer Lawrence\ Lessig\ -\ Free\ Culture.epub cover.png 128
    {% endhighlight %}

will look into the epub to find its cover, and will generate a 128px png file (named cover.png)
