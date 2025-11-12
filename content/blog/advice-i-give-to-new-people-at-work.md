---
title: Advice I give to new people at work
date: 2025-11-11
tags: work
---

Standard disclaimer: probably boring if you're not a software engineer, and may apply differently at companies with different cultures than mine.

1. **Focus on shipping as much code as you can.**
	1. Code review is an educational medium. You might publish a single diff and get five comments, each of which teaches you a key new concept about how code is written and deployed at our company.
	2. Shipping code exercises all the major engineering skills you want to build during ramp-up. And if you aren't shipping much code, it's a useful signal to look at what's slowing you down, and fix it: do you need to get better at searching through existing code? Are you spending too much time blocked before asking for help? Is your build taking hours because no one's told you the standard command? etc.
2. **Write small diffs, and publish them early.**
	1. If you're not totally sure about your approach, just call out any open questions or uncertainties in the summary. Better to get advice early rather than spending hours building confidence in your approach, just to publish and have someone point out a different, better approach that you simply had no idea about because you're new.
3. **Learn just-in-time.**
	1. Don't try to study ahead of time wikis that seem like they'll be useful to know -- you'll guess wrong about what will be relevant later, and you'll forget the relevant stuff by the time you need it anyway. Instead, ramp up by working on concrete tasks, and learn just-in-time by reading exactly the resources necessary to complete the task.
4. **While you're new, bias toward asking for help sooner when you get stuck.**
	1. Yes, there's a lot of value in struggling through on your own, but it diminishes rapidly after 30 minutes to an hour. After that point you maximize learning by just asking for help, learning something from the answer you get, and moving onto the next task.
5. **Start reviewing code as soon as you can. You'll learn a ton from doing so.**
	1. You can gradually get your feet wet. Start by just reading diffs by teammates as they come up for review - pay attention to what they're working on, how they write the code, how they write their summaries and test plans, and what comments other people leave on the diff - you'll learn a ton from this.
	2. Soon you can start leaving non-blocking comments on the diffs. If something isn't clear, e.g. you don't understand why a particular code block is necessary, comment asking about it. You might have noticed a real issue, or at least an ambiguity that could confuse other reviewers. And even if not, you'll learn by getting your questions answered.
	3. Then when you feel comfortable, start accepting or requesting changes on diffs that you feel like you have enough context to safely review, and over time (and as you become more ramped up) work your way up to reviewing more complex changes.
6. **Stay busy by parallelizing tasks *and* parallelizing your asks for help.**
	1. You could work on one task until you get stuck, then ask for help, then wait until your question gets answered, then continue work on your task.
	2. OR: you can work on Task A until you get stuck, then ask for help. Then work on task B while waiting for an answer. And this is infinitely scalable! If you get stuck on task B while you still haven't heard back on task A, ask for help on task B, then start working on task C. At some point one of your requests will get answered, and you can circle back to that task and push it forward until it's complete or you're stuck again - then rinse and repeat.
	3. This basically earns you free additional throughput: if it would have taken you six hours to debug A by yourself, but you asked for help and were able to spend those six hours working on B while you waited, then you will accomplish in six hours what would have taken you twelve hours otherwise. And again - this keeps multiplying as you work on tasks in parallel. Very powerful!
	4. Also, prioritize following up on support requests over doing new work.  So in the above situation, if you're working on task B when someone responds to you on task A, try to pause work on B and get back to that person as quickly as possible. There's often a back-and-forth necessary to resolve the issue, meaning the long pole for you completing the task will be the communication latency on either end - and you can at least minimize the latency on your end.
7. **Write posts about what you do.**
	1. Built something cool? Post a demo video. Improved a tool? Tell the team about the improvements. Debugged something interesting? Post about your process and what you learned. Need help from a framework team? Post in their support group. Most people don't post enough, but it's super important and the primary communication mechnanism at our company. Posting helps you get unblocked (it's significantly *better* than chat for asking questions in many cases, since many people might see your post and answer, vs. just the one person you pinged in chat); your posts become searchable documentation for yourself and others; your posts build your reputation; and often the post itself is *impactful* because of the knowledge it spreads.