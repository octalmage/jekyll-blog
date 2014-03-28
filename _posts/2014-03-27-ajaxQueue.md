---
layout: post
title: "ajaxQueue"
---

While working on the Now Playing page for YouParty I needed a way to have a bunch of ajax requests made in order. When a user opens the page it requests the current queue from the server, then the client needs to get the title, views, likes, and description for the video from YouTube. I ran into some issues with the requests finishing at different times then displaying out of order. Luckily I came acrosss a bit of code called [ajaxQueue](https://github.com/gnarf/jquery-ajaxQueue) that has the same syntax as the jQuery ajax function but it queues the requests. This was exactly what I needed and it works great