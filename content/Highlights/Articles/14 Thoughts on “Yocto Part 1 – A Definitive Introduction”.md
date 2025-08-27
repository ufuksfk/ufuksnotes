---
draft: true
description:
socialDescription:
title: 14 Thoughts on “Yocto Part 1 – A Definitive Introduction”
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
author: [[Shashank Kulkarni]]
url: https://kickstartembedded.com/2021/12/19/yocto-part-1-a-definitive-introduction/

last highlighted date: [[2024-06#10]]

## Highlights
- As a *vehicle for users to download Yocto* Project. Poky is **not** *a product level distro*, but a good starting point for customization. Poky is an integration layer on top of oe-core.
- They are stored in *layers*. In fact, the layered nature of Poky is what makes it extremely scalable, versatile and easy to adapt to a variety of systems. For example, you will have all recipes pertaining to networking in one layer, all recipes related to your application in another, a dedicated layer for your graphics subsystems, and so on!
- Bitbake is a scheduler and execution engine which *parses* instructions (recipes) and configuration data. It then *creates a dependency tree* to order the compilation, *schedules* the compilation of the included code, and finally, *executes the building* of the specified, custom Linux image (distribution). BitBake is a make-like build tool.
    - Note: bitbake
- So, we get it. There are a *lot* of components that play a significant role in the creation of the image? But what does the overall workflow look like? Let’s find out.
- ![](https://i0.wp.com/kickstartembedded.com/wp-content/uploads/2021/12/yp-how-it-works-new-diagram-1.png?resize=1100%2C511&ssl=1)
- **Step 4:** What do you do with source code? You build! That indeed is the next step. Most common build tools like autotools, cmake, etc. are supported. Bitbake takes care of doing the necessary configuration and compilation.
- By the way, a linux image is not all that the build process can create. The build process can also optionally be used to generate an SDK that can be used to develop and build applications for the machine that is running the very image you generate and load on that machine. This is extremely handy and takes away tons of complications that may result from not using a tailored SDK – especially in a diverse team of developers!
