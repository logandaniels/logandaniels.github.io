---
title: What is a Like, anyway?
date: 2024-09-21
tags:
---

I often Like something on a social media platform to support the creator of the content. It's not that I necessarily enjoyed viewing it, but instead that I want *other* people to see that content. Or it's not that I necessarily want to see more of that content, but I do want to give feedback to the creator that they should keep making content like that.

It's a subtle difference, but it actually matters quite a bit. I enjoy viewing things that teach me something new, or expose me to ideas I haven't heard before. If I Like something because it espouses a viewpoint I already hold, and the algorithm learns that it should therefore show me more content promoting viewpoints I already hold, that's the exact opposite of what I want.

It comes down to the semantics of a Like. What does a Like mean? Does it always mean the same thing to each person? And how differently is it used by different people?

On Reddit, there's no consensus over what the upvote and downvote buttons should mean, and many subreddits even add custom hover text to override the meaning of the buttons. For example, one I just checked suggests you should downvote if "This comment is irrelevant, misleading or nonsensical." A separate subreddit's downvote hover text reads "For content that does not contribute to any discussion."

It's even trickier when there are multiple ways to give feedback on something. For a while Amazon let me either "heart" a product, or "save" a product, and it wasn't clear what the difference was[^1]. 

Facebook offers seven different reaction types, each keyed to a universal human emotion, which reduces overloading of the Like semantics while also avoiding varying interpretations.

The website [LessWrong](https://www.lesswrong.com/posts/ByqKwsYK6rH6AYNDY/reacts-now-enabled-on-100-of-posts-though-still-just) takes reaction types to the extreme, offering so many reaction types, from "Misunderstands position?" to "I put about 75% likelihood on this claim", that they offer search feature in the reaction UI. This is all in addition to an overall post up- and down-voting system, where they made what I consider a genius move by separating overall Karma ("How much do you like this overall?") and Agreement ("How much do you agree with this, separate from whether you think it's a good comment?").

### Does it matter?
If your definition of a Like is very different than other people's definition of a Like, I think any content ranking algorithm will treat you like the average user and interpret your actions accordingly, so you'll probably get mis-targeted as a result of your eccentricity. In theory it shouldn't be a problem that there are multiple actions (like Amazon's heart and save), as the algorithm should just infer the semantics of each one separately. But this probably introduces a higher likelihood that the way you use heart or save is different than the average user, maybe exacerbating the eccentricity penalty[^2]. 

For websites with karma systems, it's important not just that voting actions align with the type of content people should be incentivized to post, but also that *everyone is on the same page* on what those actions mean. Splitting out action types a la LessWrong is a great way to disentangle actions that are over-aggregated, at the cost of increased complexity (and probably some drop-off in total votes due to the complexity).

Aside from the more easily understood impacts, I'd guess there are **significant** differences -- not easily explicable, as they are trapped in the black box of machine learning -- to the health and content ecosystem of any platform as a result of the feedback mechanisms they provide.

I wonder where we'd be -- as a society! -- if the standard reaction type for websites were not Like or Love, but "dang that's cool". Or if upvote and downvotes were universally "this is new to me" and "heard that one before". Or would we inevitably just converge on cultural norms that distill everything down to Likes and up/downvotes anyway?



[^1]: They seem to have consolidated on just "heart" now, thankfully.
[^2]: Unless some critical threshold is crossed such that "when everyone's eccentric, no one is"?