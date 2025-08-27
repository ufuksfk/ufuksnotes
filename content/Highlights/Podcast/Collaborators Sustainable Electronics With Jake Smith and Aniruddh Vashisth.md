---
title: "Collaborators: Sustainable Electronics With Jake Smith and Aniruddh Vashisth"
draft: true
tags:
  - highlight/podcasts
date: 2025-08-24
modified: 2025-08-24
---
author: [[Microsoft Research Podcast]]
url: https://share.snipd.com/episode/bae8af8b-e486-4e28-a1a3-0350eaac2a80
last highlighted date: [[2025-W34#0]] 2025-08-24
published date: [[]]

## Highlights
- **Sustainable Polymers**
  - Jake Smith and Anirud Vashist are using machine learning to design sustainable polymers. 
  - Their project focuses on printed circuit boards (PCBs). [[(PCB) Printed Circuit Board]]
  Transcript:
  Gretchen Huizinga
  With Dr. Jake Smith, a senior researcher at Microsoft Research and part of the Microsoft Climate Research Initiative, or MCRI. And with him is Dr. Anirud Vashist. He's an assistant professor of mechanical engineering at the University of Washington and director of the Vashist Research Lab. Jake and Anirud are working on a project that uses machine learning to help scientists design sustainable polymers with a particularly exciting application in the field of the ubiquitous Printed circuit board, or PCB. But before we get all sustainable, let's meet our collaborators.
- **Jake's Career Path**
  - Jake Smith initially focused on basic chemistry, studying atomic interactions, then transitioned to applied research, including modifying proteins and drug design.
  - He joined Microsoft to explore using DNA for digital data storage due to its long-lasting properties.
  Transcript:
  Jake Smith
  And so I did a couple of postdocs, first looking at how we can more effectively modify proteins after we've synthesized them so they might have a property that we care about, and then Later doing similar work on small molecules in a more traditional drug design sense. But after I finished that, I wound up here at Microsoft. We were very interested in one molecule in particular, or one family of molecules, which is DNA, and we wanted to know, how do we make DNA at just gigantic scale so that we can take that DNA and we could store digital data in it? And because DNA has this nice property that it kind of lasts forever, at least on our human scale, it makes a very nice archival storage medium. So we worked on this project for a while and at some point we determined we can kind of watch it blossom and find the next challenge to go work on.
- **Polymer Types**
  - Polymers are thermosets (set network) or [[thermoplastics]] (sliding noodles). 
  - [[Vitrimers]] combine flowability with the ability to unclick and reclick at a molecular level, enabling reprocessing and longer lifecycles.
  Transcript:
  Aniruddh Vashisth
  But in general, we have been super, super excited and interested about sustainable polymers, making sustainable composites. Particularly, we are very excited and interested in Wittremer polymers. So let me just take a step back. I'll probably wear my professor hat straight over here. Yeah, let's do. Let's go. And I'll tell you just like taking a step back, what are the different types of polymers? So in general, you can think of polymers as thermosets or thermoplastics. So to Jake's point, let's just go to the molecular scale there. And you can think of polymers as a bunch of these pasta noodles, which can slide over each other, right? Or these bunch of pasta noodles, which are packed together. So thermoset, as the name suggests, it's a set network. The pasta noodles are kind of like set in their place. Thermoplastics is when these pasta noodles can slide over each other. So you probably put too much sauce in there. Yeah, so a good analogy there would be a lot of the adhesives that we use are thermosets because they set after a while. Thermoplastic, we use plastics for 3D printing a lot. So those are thermoplastics. So they are solid. You can heat them up. You can make them flow, print something, and they solidify. Murtumas are very exciting because just like thermoplastics, they have this flowability associated with them. But more at a molecular scale, like if you think of a single pasta noodle, it can unclick and reclick back again. So it's made up of these small Lego blocks that can unclick and reclick back. Lego pasta. Lego pasta. I like that. Exactly. So this unclicking and reclicking can make them reprocessable, reusable, recyclable. Gives them like much longer life because you can heal them. And then Wittemers basically become the vampires of the polymer universe. Meaning they don't die? Well, they have like much longer life.
- **Ubiquitous PCBs**
  - PCBs are found everywhere, from [[laptop]]s and mics to automobiles and medical devices.
  - Their composition varies based on the end application, featuring stiff inclusions in a polymeric matrix with electronics on top.
  Transcript:
  Gretchen Huizinga
  Anirud, sticking with you for a minute, before we get into the collaboration, let's do a quick level set on what we might call the secret life of circuit boards. For this, I'd like you to channel David Attenborough and narrate this PCB documentary. Where do we find printed circuit boards in their natural habitat? How many species are there? What do they do during the day? How long do they live? And what happens when they die?
  Aniruddh Vashisth
  Okay, so do I have to speak like David? Yes, I'd appreciate it if you try. No, be your voice. Yeah. Yeah. So PCBs are, if you think about it, they are everywhere. PCBs are in these laptops that we have in front of us. Probably there are PCBs in these mics, automobiles, medical devices. So PCBs are, they're just like everywhere. And depending upon what is their end applications, they have a composite part of it to where you have some sort of a stiff inclusion in a polymeric matrix, which is holding this part together And has a bunch of electronics on top of it. And depending on the end application, it might come in different flavors, something that consists in much higher temperatures, something which is flexible, things of that sort. And they live as long as we use the material for, like, you know, as long as we are using these laptops or as long as we end up using our cars.
- **Ubiquity and E-waste of PCBs**
  - Aniruddh Vashisth explains that printed circuit boards (PCBs) are ubiquitous, found in laptops, mics, automobiles, and medical devices.
  - Unfortunately, there is a lot of e-waste created, with about 50 million metric tons generated every year. [[Numbers related to ESG]] [[Circular Economy]]
  Transcript:
  Aniruddh Vashisth
  So PCBs are, they're just like everywhere. And depending upon what is their end applications, they have a composite part of it to where you have some sort of a stiff inclusion in a polymeric matrix, which is holding this part together And has a bunch of electronics on top of it. And depending on the end application, it might come in different flavors, something that consists in much higher temperatures, something which is flexible, things of that sort. And they live as long as we use the material for, like, you know, as long as we are using these laptops or as long as we end up using our cars. And unfortunately, there is a lot of e-waste, which is created at the end. There's been a lot of effort in recycling and reusing these materials, but I'm confident we can do more. Right. I think there's like close to 50 million metric tons of e-waste, which is generated more than that, actually, every year.
- **Circular Economy Vision**
  - Microsoft's climate research initiative envisions a circular economy to minimize the use of non-renewables.
  - The project with Aniruddh focuses on recapturing unavoidable materials, driven by the need to capture and reuse [[Carbon dioxide]].
  Transcript:
  Gretchen Huizinga
  So right now, are they sort of uniform, the printed circuit board? I know we're going to talk about Vitrimer-based ones, but I mean, other than that, are there already multiple materials used for these PCBs? Jake, you can even address that.
  Jake Smith
  Yeah, of course. So there are kind of graded ranks of circuit board materials that, as Anna Reid said, might be for specialty applications where you need higher temperature tolerance than normal, Or you need lower noise out of your circuit board. But kind of the bog standard circuit board, the green one that you think about if you've ever seen a circuit board. This is like a anti-flammability coating on a material called FR4. So FR4, which is an industrial name for a class of polymers that are flame retardant, thus FR. And four gives you the general class. This is the circuit board material that, you know, we really targeted with this effort.
  Gretchen Huizinga
  Interesting. So, Jake, let's zoom out for a minute and talk about the big picture and why this is interesting to Microsoft research. I keep hearing two phrases, sustainable electronics and a circular economy. So talk about how the one feeds into the other and what an ultimate success story would look like here. Absolutely.
  Jake Smith
  So I'll start with the latter. When we set out to start the Microsoft Climate Research Initiative, we started with this vision of a circular economy that would do things that avoid what we can avoid using, but there Are many cases where you can't avoid using something that is non-renewable. And there, what we really want to do is we want to recapture what we can't avoid. And this project falls in the latter, and there's a lot of things that fall in the latter case. So, you know, we were looking at this at a very carbon dioxide centric viewpoint where CO2 is ultimately the thing that we're thinking about in the circle. Although you could draw a circular economy diagram with a lot of things in the circle. But from the CO2 viewpoint, you know, what led us to this project with Anarut is we thought we need to capture CO2. But once you capture CO2, what do you do with it? You can pump some of it back into the ground, but this is an economically nonproductive activity.
- **Upcycle CO2**
  - Upcycle CO2 into something useful to replace existing materials.
  - Reduce e-waste by replacing FR4 with atoms from captured CO2.
  Transcript:
  Jake Smith
  We upcycle the CO2 into something interesting. And what we really want, and what we still really want, is to be able to take that CO2, convert it down into a useful chemical feedstock, and there are great laboratories doing work on This. And then we could, you know, look at our plastic design problem and say, hey, we have all this FR4 in the world. How could we replace the FR4, you know, explicit atoms that are in the FR4 with atoms that have come from CO2 that we pulled out of the air. And so this is the circular economy portion. We come down to, you know, the specific problem here. Andrew talked a lot about e-waste. I had great colleagues who also collaborated with us on this project, Bicklinda Wynn, Kelly Frost, who have been doing work with our product teams here at Microsoft you know, what can We do to reduce the amount of e-waste that they put out towards Microsoft's climate goals?
- **AI for Science**
  - Microsoft's AI for Science initiative aims to accelerate research. The vitrimer-based PCBs project became part of it a year or two after the collaboration started.
  Transcript:
  Gretchen Huizinga
  So the University of Washington and Microsoft meet again. Well, Jake, let's do another zoom out question, because I know there's more than just the Microsoft Climate Research Initiative. This project is a perfect example of another broader initiative within Microsoft, which has the potential to, quote, accelerate and enhance current research. And that's AI for Science. So talk about the vision behind AI for Science. And then if you have any success stories, maybe including this one, tell us how it's working out. Yeah, absolutely.
  Jake Smith
  We are, and by we, I mean myself and my immediate colleagues are certainly not the only ones interested in applying AI to scientific discovery at Microsoft. And it turned out a year or two after we started this collaboration, a bigger organization named AI for Science, arose and we became part of it.
- **Economic Incentives Over Consumer Behavior**
  - Shift focus from individual consumer behavior to economic incentives for large-scale actors.
  - Adding economic value to waste material can drive reusability and reduce e-waste.
  Transcript:
  Gretchen Huizinga
  Because it's convenient and you can take it in your car and not spill. Agreed, yes.
  Jake Smith
  I also have this cup and it could not spill as well. True, reusable. No, no, this is like a, it's an ingrained consumer behavior that I've developed. I'll slip into Jake's personal perspectives here, which is that it should not be on the individual consumer behavior changes to ultimately drive a shift towards reusable and recyclable Things. And so one of the fundamental hypotheses that we had with the design of the projects we put together with the MCRI was that if we put appropriate economic incentives in place, then we Can naturally guide behavior at a much bigger scale than the individual consumer. Maybe we'll see that trickle down to the consumer, or maybe this means that the actual actors, the large-scale actors, then have the economic incentive to follow it themselves. So with the e-waste question in particular, we talked a lot about FR4, and it's the part of the circuit board that you're left over with at the end that there's just nothing to do with. And so you toss it in a landfill, you burn it, you do something like this. But, you know, with a project like this, where our goal was to take that material and now make it reusable, we can add this actual economic value to the waste there.
- **Vitrimer PCB Prototype**
  - A prototype vitrimer-based circuit board was created in collaboration with Vikram Eyer's lab.
  - The prototype functions as expected and can be disassembled and reassembled.
  Transcript:
  Gretchen Huizinga
  So would you say that the Vitramer-based printed circuit board is a proof of concept right now or have you made prototypes? Where is that now? Yeah, absolutely.
  Jake Smith
  We've mentioned our other collaborator, Vikram Eyer, a couple of times. And in collaboration with his lab, we did actually make a prototype circuit board. We showed that it works as you expect. We showed that it can be disassembled, it can be put back together, and it still works as expected. The break stuff makes stuff. But, you know, I think to the spirit of the question, it's still individual kind of one-off experiments being run in a lab, and Anirud is right. There's a long way to go from like a technology readiness level three, where we're doing it ourselves on bench scale up to, you know, the seven, eight, nine, where it's actually commercially Viable when someone has been able to reproduce this at scale.
