---
title: Embedding Open Street Map
author: Andy Choens
layout: post
category: Etc.
excerpt: For one of my many projects, I've been trying to embed some mapping content and it looks like OpenStreetMap may be the answer I'm looking for.

---

For one of my many projects, I've been trying to embed some mapping
content and it looks like OpenStreetMap may be the answer I'm looking
for. For example, the Albany Museum of History and Art which is at:

125 Washington Avenue Albany, NY

I can link to the page, [easily](http://www.openstreetmap.org/way/89868754).

I can also embed things pretty easily (I think).

    <iframe width="425" height="350" frameborder="0" scrolling="no" marginheight="0" marginwidth="0" src="http://www.openstreetmap.org/export/embed.html?bbox=-73.76126557588577%2C42.65529619325159%2C-73.75997811555861%2C42.65638506618383&amp;layer=mapnik" style="border: 1px solid black">
    </iframe>
    <br/>
    <small>
        <a href="http://www.openstreetmap.org/#map=19/42.65584/-73.76062">View Larger Map</a>
    </small>

Which results in this:

<iframe width="425" height="350" frameborder="0" scrolling="no" marginheight="0" marginwidth="0" src="http://www.openstreetmap.org/export/embed.html?bbox=-73.76126557588577%2C42.65529619325159%2C-73.75997811555861%2C42.65638506618383&amp;layer=mapnik" style="border: 1px solid black">
</iframe>
<br/>
<small>
    <a href="http://www.openstreetmap.org/#map=19/42.65584/-73.76062">View Larger Map</a>
</small>

This is, of course, blocked, because of concerns about iframes.
