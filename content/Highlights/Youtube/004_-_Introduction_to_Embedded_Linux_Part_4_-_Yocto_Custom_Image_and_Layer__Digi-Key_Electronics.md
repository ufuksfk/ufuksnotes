---
draft: true
description:
socialDescription:
title: 004_-_Introduction_to_Embedded_Linux_Part_4_-_Yocto_Custom_Image_and_Layer__Digi-Key_Electronics
  | Digi-Key Electronics
tags:
- highlight/youtube
date: 2025-05-18
modified: 2025-08-21
---
https://www.youtube.com/watch?v=bTEdfwtPtNY&list=PLEBQazB0HUyTpoJoZecRK6PpDG31Y7RPB&type=snipo

[[DigiKey]]


![Untitled](Untitled%20853.png)

## how to source

## how to create a layer:

[7:28](https://www.youtube.com/watch?v=bTEdfwtPtNY&list=PLEBQazB0HUyTpoJoZecRK6PpDG31Y7RPB&index=4&t=449s&type=snipo)
The bsp layer the pokey layer and then you combine all of those in your build process locally to create your image we're going to use the bitbake layers command and we're going to create a layer this is going to be our custom layer and most layers you will find start with the meta prefix so we're going to call 
 

![Untitled](Untitled%20854.png)

## how to steal minimal image:

![Untitled](Untitled%20855.png)

inherit is like import

![Untitled](Untitled%20856.png)

[12:49](https://www.youtube.com/watch?v=bTEdfwtPtNY&list=PLEBQazB0HUyTpoJoZecRK6PpDG31Y7RPB&index=4&t=770s&type=snipo)
It's generally advisable to let it expand to the space that's needed but i'm showing you here how you can create a larger root file system to give you more space available when you install linux on your root file system now for security purposes you generally want to have a root file system that's just big enough for your kernel packages other modules libraries that you need to get your 
 

## ?= vs =

[14:54](https://www.youtube.com/watch?v=bTEdfwtPtNY&list=PLEBQazB0HUyTpoJoZecRK6PpDG31Y7RPB&index=4&t=894s&type=snipo)
Allowing somebody to make changes in the build directory say remember that build conf local.conf file that we could modify somebody could change these variables there if they wanted to create a different route file system size or assign a different root file system size in order to say expand it to the full extents of whatever sd card they have 
 

![Untitled](Untitled%20857.png)

adding a new layer to bblayers.conf

![Untitled](Untitled%20858.png)

![Untitled](Untitled%20859.png)

bitbake -e means you are searching

you can have a conflict for usermod, so search for IMAGE_FEATURES and close conflicting ones