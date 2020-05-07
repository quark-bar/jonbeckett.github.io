---
layout: page
title: Podcast
permalink: /podcast/
image: https://source.unsplash.com/VCFxt2yT1eQ/1200x800
---

When not writing blog posts, I record conversations with bloggers all over the world about their journey - their earliest memories of using the internet, how they started blogging, what their motivations are, their insiprations, and where they think they might go next.


## Finding the Podcast

The podcast is published to [Anchor.FM](https://anchor.fm/jonbeckett), then syndicated to the following services:

* [Spotify](https://open.spotify.com/show/1oyFiYa5ksHXazlpHtuznB)
* [Apple Podcasts](https://podcasts.apple.com/gb/podcast/jonathan-becketts-podcast/id1495777447)
* [Google Podcasts](https://podcasts.google.com/?feed=aHR0cHM6Ly9hbmNob3IuZm0vcy8xNDFjODcwYy9wb2RjYXN0L3Jzcw&ved=0CAAQ4aUDahcKEwjAqqC3rfXnAhUAAAAAHQAAAAAQCQ)
* [TuneIn](https://tunein.com/podcasts/Arts--Culture-Podcasts/Jonathan-Becketts-Podcast-p1287145/)
* [Facebook](https://www.facebook.com/jonbeckettpodcast)

## Getting on the Podcast

If you have a blog, or an internet story you would like to share, get in touch via the contact page.


## Recent Episodes

<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.4.1/jquery.min.js"></script>

<script type="text/javascript">

$(document).ready(function(){
    var feed = "https://anchor.fm/s/141c870c/podcast/rss";

    $.ajax(feed, {
        accepts:{
            xml:"application/rss+xml"
        },
        dataType:"xml",
        success:function(data) {

            $(data).find("item").each(function () { 
                var el = $(this);
                
                $("#recent").append("<h3><a href='" + el.find("link").text() + "' target='_blank' title='" + el.find("title").text() + "'>" + el.find("title").text() + "</a></h3>\n<img src='" + el.find("itunes\\:image").attr("href") + "' style='float:right;max-width:200;max-height:200;padding-left:20px;padding-bottom:50px;' width='150' height='150' /><p>" + el.find("description").text() + "</p><p>" + el.find("pubDate").text().substr(0,16) + "</p>\n<div style='clear:both;'></div>\n<hr style='border:0px;border-bottom:1px solid #ddd;width:50%;margin:auto;padding-top:10px;padding-bottom:10px;' />\n");

            });

        }	
    });
});
</script>
<div id="recent"></div>


## Supporting the Podcast

If you would like to support the podcast, you can do so via [PayPal](https://paypal.me/pools/c/8nIZt2ZDMp). All contributions are gratefully received.
