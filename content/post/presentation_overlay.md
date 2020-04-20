+++
date = "2020-04-20T14:45:00"
draft = false
tags = ["blog", "OBS", "overlay"]
title = "Presentation Overlay"
math = true
summary = "How to use OBS to overlay your presentation on your webcam image."

[header]
image = "headers/layers.png"
caption = "Layers"

+++

So, the webinar on distance assessment was received quite well. Apart from the 200 attendees and now almost a hundred views on YouTube, I also received many questions on how I created the presentation overlay.

<iframe width="560" height="315" src="https://www.youtube.com/embed/wzMtb3vFJm4?start=2461" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## All about the layers

To create this effect, I stacked some video layers and applied some chroma-keying to make it all look smooth. For this, I used the opensource open broadcast software called [OBS studio](https://obsproject.com). The three essential layers needed are, of course, the webcam middle layer, a white image background layer, and the presentation layer, which is a PowerPoint with a chroma-key (green) background.

In OBS you need to set the webcam layer's opacity to 70%, and you will get a more transparent image. To add the Powerpoint overlay, [set Powerpoint to windowed mode](https://superuser.com/questions/865094/how-can-i-view-a-powerpoint-slideshow-in-windowed-mode-ie-not-full-screen) and window [capture this window in OBS](https://youtu.be/1V9rxexjyXU?t=615). NerOrDie will show you all options there are available in OBS sources.

In the final step, you just need to select a [second monitor as output in OBS](https://obsproject.com/forum/threads/preview-output-on-second-monitor.112853/) and use this second monitor as input for your conferencing software like zoom, meets, or teams. Well, here you go. 

