---
layout: post
title: Availability heurstics
category: cognitivebias
---

__(A)__ Should you be scared of a shark attack when swimming? (given the likelihood, no -- see evidence [here](?))

Instead of answering the question (__A__) properly, your brain, you, swaps it out for an easier question. __(B)__ Can I recall an image of a shark attacking a person? <span id="mouseOver"><img height="100" width="1600" src="http://4.bp.blogspot.com/-PnWxMaXSYqA/UI6BVbztxRI/AAAAAAAAMas/sKxWQ_SMIq0/s1600/Shark+Wallpapers+7.jpg">Fuck that.</span>

Why do we do this? Question __(A)__ is a hard computational question. Infact, it would require you to search through your entire memory, indexing every time you have been in the ocean or seen others in the ocean, heard some news about a shark attack, ... to recall attacks by sharks.

_This requires you to at least perform $\mathcal o(n)$ calculations to aggregate the number of ... Now you need to normalise them to get a likelihood, recalling every time you were in water, someone was in water, ... to get an estimate of_

Instead, of collecting all the proper evidence we can recall, it is far easier to generalise from one mental image. (also related to risk adversity, save compute by just avoiding all risky things period rather than trying to evaluate them accurately)

You might think that we could precompute the answers and store these facts. But this would require a large amuount of space. So we can compress these facts. A nice way of compressing this fact might be to store sharks with other scary looking beasts. Thus taking us back to where we started...

 What about getting the answers from a trusted oracle? Well they will still have exactally the same computational issues. But now, the memory complexity is shared over many people. (but now we have added another type of complexity, communication. ) 
