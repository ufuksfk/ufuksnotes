---
draft: true
description:
socialDescription:
title: PCB Prototype With Small 0.35mm Pitch BGA Chip
tags:
  - highlight/articles
date: 2025-06-21
modified: 2025-08-21
---
author: [[EEVBlog]]
url: https://www.eevblog.com/forum/eda/pcb-prototype-with-small-0-35mm-pitch-bga-chip/
last highlighted date: [[2025-06#18]]

[[PCB Design Notes]]
## Highlights
- I've contacted JLCPCB support and they said 0.35mm pitch BGA is possible, and suggested I could use in pad vias (which they can do), but given the minimum via drill and annular ring (0.2, 0.35) that seems impossible (pad INT2 in the screenshot).
- NextPCB claims to do laser blind vias.
- this is a flip chip for cell phone and tablets apps. VIPPO and ELIC process. Laserdrilled and 1/4oz copper on glass-free substrates. Apple / Samsung do this all the time. Mass production technology.
- I heard of VIPPO (Via in Pad Plated Over) but ELIC (Every Layer Inter Connect) was new to me. After some more reading it looks like it is a lot like LTCC (Low Temperature Co-fired Ceramic) but without the ceramic.  ![:D](data:image/webp;base64,UklGRowBAABXRUJQVlA4TIABAAAvDoADED/COpJkJfdwd8g/Nr7c9aR4aTCMJNnUfttW/un8SJ7fN9hGtq3kPfx/PKQAeqNdUgjd3e3NfwCA/imhdyLCGLwK7AQ4FuN+NnMJXYgddwKcFUPAV0HcQYUB4iQH0P7m/gEaCM4PQoIb8Tdif5IJSB7i7arnRPpjIk9m95vcuOHv61aPYahs20ASJIVBba6ssRna1PqBZ9NcD4M7AEXYQnIR42PsAJm/wbUNtsX90vXxm/iji/7AruFOvkOkMbh2Au/ie1EzATv+mAZjQOFHG4PD2LZN536bsW3bzkv6r+knPZwb0f8JIADd93oB0aHfXHUsgGviB7cUOam0BIBlQ1U0lVljtbQhTH0Lx73VuVjwZ7TNBzZuZ/v4sBGUdiKbcZ3X2V3fXS+T+4gMp4M6o1VDJsdilS18gRfweHI+t+qU0q/DCLrJh2Om3KFlanw3JGBwy2cWhE41VXmcetdLMV3tELCtxuGkgiiubSjZn1eaQGXZp7/DzqY9pCQ= "Cheesy")
