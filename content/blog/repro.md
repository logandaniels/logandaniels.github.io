---
title: Does it repro?
date: 2024-09-10
tags:
---

### The birds and the bees of reproduction
In software engineering, a repro is a thing of power.

A **repro** (short for reproduction) is a list of preconditions and steps taken that will produce a particular outcome.

Suppose you make an app, and your users report that your app randomly crashes. If you have a **consistent repro** -- steps that you can consistently use to trigger the app to crash -- you will almost always be able to fix the issue. Even if you can't come up with a hypothesis of why the app is crashing, you can just keep changing things around and eliminating variables until eventually the repro stops reproducing. Then whatever you just changed is the fix to the issue. Hooray!

But what if whenever you try using the app, it *never* crashes. What will you do? Even if you make a fix, you'll have no idea whether it actually worked or not, since you couldn't reproduce the problem to begin with.

And if a single person reports their app randomly crashes, but you can't reproduce it, should you actually spend time trying to fix it? Maybe their phone was in a once-in-a-lifetime bad state, and it'll never crash again. Without knowing what circumstances trigger the issue, it's hard to know how severe the issue is, or whether it is truly an issue at all.[^1]

Because of all this, a repro is worth its weight in gold. A repro can make the difference between a bug being promptly fixed, vs. a bug persisting for years.

### Reproducing other things
The key to a repro is that as long as you can reproduce an issue, you will eventually be able to fix it. So how about other issues in our lives?

Take depression as an example. Maybe every once in a while you go through a month of mild depression, and it sucks. You enact some lifestyle changes -- you start running a few times a week and supplementing Vitamin D[^2]. How do you know if it worked? If a few months go by and you don't get depressed, does that mean your interventions worked, or have you just not been experiencing whatever conditions lead to your periodic depression?

We tend to put a lot of effort into making changes to improve something, but could we put more effort into making the root issue consistently reproducible? Or even just paying careful attention to all the existing significant variables, to see which comprise the preconditions for reproducing the issue?

By this logic, Seasonal Affective Disorder should be easier to treat than a periodic depression, because the repro case is clear: wait until the middle of January. If depressed, SAD treatment unsuccessful. If not depressed, SAD treatment successful.

The [elimination diet](https://www.fammed.wisc.edu/files/webfm-uploads/documents/outreach/im/handout_elimination_diet_patient.pdf) is a great application of this principle: you remove a bunch of candidate foods from your diet entirely, then add them back one by one to see which specific food causes your symptoms when consumed. This is exactly like how you'd isolate repro steps for a software bug.

Where else can we spend more time looking for repros?



[^1]: It also becomes tempting to assume that the person reporting the crash is actually wrong -- their app *isn't* crashing, they just are interpreting normal behavior as a crash, or they're using last year's version of the app, or some other reason. A bug reporter has little credibility without a repro -- but with a repro, they are unstoppable.
[^2]: Even though the available evidence suggests that unless you're deficient in Vitamin D, supplementing it is unlikely to improve your depression.