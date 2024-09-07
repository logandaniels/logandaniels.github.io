---
title: Against PINs
date: 2024-09-06
tags:
---

Here are some places we use PINs:
* ATM withdrawals
* Mobile phone passcode
* Every random app or business that for some reason asks you to set a PIN for access

Do you see the problem?

A debit card can easily be lost or stolen. At that point, your PIN is the only thing stopping someone from exfiltrating hundreds or thousands of dollars from someone's bank account. 

A mobile phone can easily be lost or stolen. At that point, a PIN is the only thing stopping someone from hijacking most of your entire life. If someone gets into your phone, they an access your email for password resets and your text messages for 2-factor auth; maybe it's even easier and they can use your PIN to access your password manager and get into all your accounts at once.

This is fine, except that **people reuse PINs**.

So WHY do we also use a PIN to secure your access to some random-ass app that you never needed secured anyhow and which probably has terrible security to protect your PIN from leaking? For many people, that leaked PIN is likely to be the same PIN they use for super-secure things like banking and their phone.

But I'm not even that worried about some app accidentally leaking your PIN; this feels like an unlikely threat vector unless you're being targeted by state actors, at which point you're screwed anyway.

The more likely, equally bad scenario is a malicious actor asking you to generate PIN just to see what you use. It goes like this:
1. (e-)Mail the victim a survey with a $50 gift card reward for submission
2. Have them input a 4-digit PIN that they'll use to verify their identity when you send the gift card later
3. Now you probably have the PIN they use for everything

### Don't people reuse passwords too?

Yes, and that does have a very similar threat profile. But it's much easier to avoid doing so.

If my go-to password is "hunter2" and I know I shouldn't reuse my password, I can use a strategy like appending the website I'm making the password for -- so I might use "hunter2google" for my google account, and "hunter2apple" for my apple account, etc. This is not great, but there are enough possible algorithms that implementing something like this may protect you from many password reuse vulnerabilities.
 
 But there are only 10,000 total possibilities for a 4-digit PIN[^1]. And if my go-to PIN is "5678", how do I adapt that in a memorable way for new usages? "Okay, the next one will be 5679, and then 5680"...? It's pretty infeasible. So I suspect most people simply reuse the same PIN everywhere.

I also think that we've done a pretty good job educating people on the importance of using different, secure passwords. But psychologically I just don't think it *feels* as high stakes when "generating" a "new" PIN in any of the myriad places that seem to ask for it.

### What should we do about it?
You could learn [advanced mnemonic techniques](https://www.goodreads.com/book/show/6346975-moonwalking-with-einstein) and use them to memorize distinct PINs for every new service that asks for one.

Or more realistically: if you're using a [password manager](https://1password.com), which you absolutely should be, just generate a random PIN store it in your manager like you would any other password.

And anyone making an app should not use a PIN for any of its security. Just use a password, or on mobile use the device's biometric authentication (e.g. FaceID) so you can avoid having to know the user's PIN at all.

[^1]: And apparently [27% of PINs](https://informationisbeautiful.net/visualizations/most-common-pin-codes/) fall into the top 20 most common 4-digit codes.