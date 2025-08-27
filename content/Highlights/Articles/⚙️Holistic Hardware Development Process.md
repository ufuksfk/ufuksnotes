---
draft: true
description:
socialDescription:
title: ⚙️Holistic Hardware Development Process
tags: []
date: 2025-03-05
modified: 2025-08-21
---
author: [[Building Hardware]]
url: https://buildinghardware.substack.com/p/holistic-hardware-development-process

last highlighted date: [[2025-03#04]]

## Highlights
- ![](https://substackcdn.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2Fc2a3056e-3ea2-413f-8c21-84b762d2d7cf_2878x1622.png)
- Product Managers may spend hours defining vision, pricing, revenue, and product requirements but then lack awareness of the difficulty to execute on design, engineering, and manufacturing. This **inability to gauge technical feasibility results in delays and non viable product scope.**
- A smartphone PM is inspired by [[Apple]]’s AR/VR device and wants eye tracking features on their new headset but doesn’t realize their team lacks the expertise to architect the circuitry and processing for the required inward facing cameras.
- A part is cracked in production and the ME proposes an ML inspection machine to catch defects because manual visual inspection is subjective. While it’s innovative, this complex equipment spend **will add to the per unit product cost**, resulting in missing profit margins
- The industrial design team at your AR/VR headset company loves premium materials and engineers love cutting edge machining. They come together to propose a headset out of glass and stainless steel. **While this is aesthetically pleasing, the added weight is nightmare for end user ergonomics and comfort**
- An electrical engineer designing a new tablet chooses an advanced chipset to optimize device performance but these new power requirements **make replacing batteries difficult for users** and require costly repairs
- What I learned was that Tesla encouraged scrappiness while [[Apple]] was meticulous and calculated. While both philosophies were catered to each company’s maturity in the market, they followed a comparable high level process for bringing hardware products to market.
- Keep in mind that build volumes and development timelines obviously vary by industry. In **automotive a new product cycle usually takes 5 years from concept to launch, while consumer electronics is about 18 months.**
- 3. Hardware Product Development Process Explained
- Phase 1 - Concept
- • The goal here is to find a sweet spot between company vision, market gaps, and user problems
- This stage cumulates with a press release (**PRFAQ**) draft document which is an artifact that looks back from the customer experience to help articulate the vision for a new product
- PRFAQs are basically a product business case and can take weeks to months to write. They’re supposed to create excitement but also balance that by answering difficult stakeholder questions (technical and financial). The how isn’t needed at this stage.
- Phase 2 - Definition
- This is where product managers are talking to customers, defining user problems, **turning problems into stories, and those user stories into a set of crisp product requirements**
- The key outcome in this phase is a **dev commit** from your entire team to start detailed design, engineering, marketing, sales, and supplier work
- Its important to remember that **product requirements are not engineering specifications**. It seems obvious but this is important context which I, and many former engineers, missed early in our careers so I feel it’s important to highlight here.
- Phase 3 - Development
- The goal here is to go from concept to **execution** and it is undeniably the most difficult part of the product development process
- The development phase is divided into sub phases or engineering builds shown below
- ![](https://substackcdn.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2F22e7add1-a2b2-40c2-b135-b23da70542fb_2048x1012.png)
- **Prototype (PT)**
  • In PT Industrial design starts ideating on their shapes, colours, materials, and form factor concepts
- The goal is to **validate the initial functionality of key features and not necessarily the entire system at once** - not all modules need to be working at the same time
- Engineering Validation Test (EVT)
- **EVT cumulates with a “pencils down”** which means design and engineering should, *in theory*, be locked
- **Design Validation Test (DVT)**
  • At DVT teams usually produce engineering designs with different suppliers for the first time to help de-risk the supply chain
- Teams also continue reliability testing & **lock product quality specs**
- Production Validation Test (PVT) & MP (Mass Production)
- This is the production ramp phase where you **stress the assembly line** to evaluate **peak volume**, max throughput, and process capability
- Ramp is often the litmus test of many engineering and process assumptions
- Alpha User Testing
- While EVT → PVT above focus on engineering development, there is user testing done in parallel to provide feedback loops on user experience
- Led by product managers the **alpha phase is typically the first time you can gain any user feedback** of a semi mature product and it typically **coincides with EVT**
- Beta User Testing:
- The goal here is to validate real-world customer usage flows and get more robust feedback
- **This requires detailed scoping from the product manager** including a systemized experimentation plan, confidentiality clauses, and more
- **Do not** rely on just a landing page or video to assume user feedback. **Customers need to** feel, interact with, wear, and physically test your product
- From the technical side engineers should be prepared for **FFA** **(field failure analysis)** to address issues which slipped through development (for example, the iPhone 6 bend gate)
