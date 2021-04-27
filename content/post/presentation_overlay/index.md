---
date    : "2020-04-20T14:45:00"
draft   : false
tags    : ["blog", "OBS", "overlay"]
title   : "Presentation Overlay"
math    : true
summary : "How to use OBS to overlay your presentation on your webcam image."

image:
  caption : "Layers"
  placement : 3
---

So, the webinar on distance assessment was received quite well. Apart from the 200 attendees and now almost a hundred views on YouTube, I also received many questions on how I created the presentation overlay as can be seen in the video below.

<iframe width="100%" height="385px" src="https://www.youtube.com/embed/wzMtb3vFJm4?start=168" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## All about the layers

To create this effect, I stacked some video layers and applied some chroma-keying to make it all look smooth. For this, I used the opensource open broadcast software called [OBS studio](https://obsproject.com). The three essential layers needed are, of course, the webcam middle layer, a white image background layer, and the presentation layer, which is a PowerPoint with a chroma-key (green) background ([Download Template](http://www.klinkenberg.amsterdam/files/Chroma_Key_PowerPoint.pptx)).

<!-- http://cogentstudios.com/how-to-set-opacity-obs-studio/ -->

In OBS you need to set the webcam layer's opacity to 40% by applying a a **color key** [filter](https://youtu.be/-aXtar17E3o?t=64), and you will get a more transparent image. To add the Powerpoint overlay, [set Powerpoint to windowed mode](https://superuser.com/questions/865094/how-can-i-view-a-powerpoint-slideshow-in-windowed-mode-ie-not-full-screen) and window [capture this window in OBS](https://youtu.be/1V9rxexjyXU?t=615). Watch [this last video](https://youtu.be/1V9rxexjyXU) entirely for all the sources options available in OBS.

In the final step, you just need to select a [second monitor as output in OBS](https://obsproject.com/forum/threads/preview-output-on-second-monitor.112853/) and use this second monitor as input for your conferencing software like zoom, meets, or teams. Well, here you go. 

So, am I satisfied? Nah, the text overlaying the eyes is just too distracting to me. I already experimented with using a half-width PowerPoint presentation, so you only use half of the screen. I'll come back to that in the next post.