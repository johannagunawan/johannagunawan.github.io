---
layout: post
title:  On the escapability of marketing emails
date:   2022-04-27 00:00:00
description: Notes from a personal experience with Xfinity's email advertisements
tags: xfinity dark-patterns opt-out email-marketing spam
categories: in-the-wild
---
_Originally from a Twitter thread._

One personal beef of mine (with the internet, of which there are many) is with email marketing. It's crazier for me to look back and realize that I used to work in digital marketing and ate up the marketing industry gospel of email engagement; yep, I once used popular tools like MailChimp and HubSpot to spam mailing lists with chirpy, 'relatable' content that encouraged clicks. Those days are behind me, though certainly quite informative, and now I'm just a grump on my digital lawn, kvetching about the exhaustive, endless slog of spam-like emails in my inbox. 

One bone I've had to pick for a while is with Xfinity, my local internet provider (not that I've got many competitive options in my area). As far as my internet goes, it's fine for my uses, and for the most part doesn't really impact my life outside of move-ins, new user registration, and move-outs. One exception to that: my inbox. 

<img src ="https://johannagunawan.com/assets/img/blog/2022-04-27-xfinity-this-is-an-advertisement-email-byline.png" width="750" />
*Xfinity at least tells you if an email is an ad; +1 to CAN-SPAM compliance, I guess.*

Now, don't get me wrong; I'll give Xfinity some credit for actually complying to CAN-SPAM's rules in saying whether an email is 'service-related' or an 'advertisement,' though I've definitely gotten promotional-content emails that have been marked as 'service related.' (Unfortunately I don't have receipts for those, as it's understandably tiring to collect screenshots of every single horrible interface I encounter). That said, that information is always in the greyed-out, deprioritized fine print at the bottom of a mega-HTML email, so I'd warrant that few people actually open up their annoying mail and scroll all the way down. I only do so for work, or when an email worms past my painstakingly developed inbox filters that STILL don't catch everything. Marketers are wily!

After a few random instances of inbox opening and aggravated sighing following the receipt of yet more Xfinity emails for products and services I do not want or need, I finally decided to spend the clicks on the unsubscribe button rather than letting the emails fester in Google's cloud storage (and subsequently, my inbox filters). 

<img src="https://johannagunawan.com/assets/img/blog/2022-04-27-xfinity-unsub-all-fineprint.png" width="750" />
*Stop getting promotional emails in 48 hours? Sign me up!*

The site initially presented me with a bunch of individual toggles -- ugh -- but I clicked on those anyway and quickly left the site. A bit of time later, I noticed I was still getting emails, so I checked back -- ugh x2 -- and went back to the unsubscribe page only to see that I'd hastily left the site the first time around; if I scrolled down, I was rewarded with a bulk toggle to opt out of EVERYTHING at once. And if I took a look at the greyed-out fine-print below that, I was rewarded with text that told me **when** I should expect the ceaseless influx of chirpy promotions to, well, _cease_. Great! I opted out, and was excited to stop seeing emails within 24-48 hours. And just to be sure, this second time around, I noted the date. February 28, 2022, I opted out of 'all email communications' on Xfinity's provided unsubscribe link. 

But the cards were not in my favor, and whatever happened in Xfinity's email system piping kept sending emails. I kept an eye on my inbox for a few weeks, opening emails to check if they were ads (yep), but realizing that MAYBE my original individual toggles were triggering that 60-day 'processing fee' for opting out under their 'new marketing preference center.' However, according back at the fine print, which is in the above screenshot taken today, I did technically flip the switch on opting out of all email communications on 2/28. Regardless of my original toggles, in theory I should have stopped getting emails by 3/2 under my interpretation of the Xfinity fine print. 

<img src="https://johannagunawan.com/assets/img/blog/2022-04-27-gmailinbox-xfinity.png" width="750" />
*Look at how many 'ADVERTISEMENT' emails I got past that 24-28 hours! The thread with 2 emails is my record of when I 'unsubscribed-all.*

Maybe there was an issue with my memory on when I had actually tried managing those individual toggles. My best estimate of when I first clicked those other toggles is around 2-4 weeks before 2/28, based on how often I actually open that inbox. Today, April 27, is 52 days after the day I hit 'unsubscribe-all,' meaning Xfinity would have 8 more days of leeway to continue sending me advertising emails if I'm being generous about their fine print and using the 2/28 date to measure their 'individual preferences effect turnaround.' But if we assume that I did toggle individual settings around 2/14, I should not be receiving that 4/21 email that triggered this all, because I definitely turned off each individual item. 

For the benefit of Xfinity's doubt and to account for my shaky memory of Unsubscribe Attempt #1, I'll keep an eye on T-60 days after 2/28 to see if maybe some wires got crossed with my multiple selections. We'll see if I'm still getting any emails after 5/5, which would be 60 days after 2/28, which is not even the correct start date from which to count to 60. 

### On user expectations
My own rudimentary experiment and data collection aside, Xfinity's fine print on expected 'off' dates for email preference processing are either buggy at best, confusing at not-so-great, or straight-up dishonored at worst. 

Specifically, the text reads: 
> As we transition to our new marketing preference center, changes may temporarily take additional time to go into effect. It may take up to 60 days to apply your individual marketing preference changes. If you've unsubscribed to all marketing communications, this will be applied within 24-48 hours.

The second sentence gives an upper bound of 60 days for individual marketing changes, which in my case is wonky due to my failure to remember when I toggled those. If I did those on the same day as 2/28 (which I know I did not), or even the day before, then fine -- in the absence of the third sentence, I should wait out around 7-8 more days and test my hypothesis again then. But if I un-checked those weeks earlier, say on 2/19, then 60 days would lead me to 2/20 and I shouldn't have received an advertising email on 4/21.

When the third sentence is accounted for, then everything goes to sh**. Firstly, it is likely unclear to users who do make it to the fine print whether the bulk opt-out toggle would override prior individual preferences. What happens if users (like me) performed both individual and bulk actions? Is, as I'm thinking, the set of individual preferences with their longer processing time considered the default if users do both? When would an option override another? Would bulk opt-out only be applied if the user NEVER touched an individual toggle? (See next section [on transparency through design](#on-transparency-through-design)).

Regardless, I did perform a bulk action (thus meeting the requirements in the third sentence) and subequently expected the opt-out to be applied within 24-48 hours. This didn't happen. What's the point of providing users with options if those options aren't effectively honored, communicated, or explicitly caveated? Is XFinity compliant with CAN-SPAM purely because they provide all these frontendy goodies (the advertisement disclosure, this fine print, and an unsubscribe portal)? (Hint: [Technically, it isn't. Yet it persists!](#on-can-spam-compliance))

### On transparency through design
Messy and confusing disclosures aside, users can't even see the bulk toggle option unless they scroll allllll the way down the page past other options. The bulk options are not provided at the top, clearly or conspiciously, and the details on when their preferences will be honored falls below all toggles at the ultimate bottom of the page. 

<img src="https://johannagunawan.com/assets/img/blog/2022-04-27-xfinity-unsub-screen1.png" width="750" />
*This is what I get on a reasonably-sized, relatively new MacBook screen when first opening an unsubscribe link.*

<img src="https://johannagunawan.com/assets/img/blog/2022-04-27-xfinity-unsub-screen2.png" width="750" />
*This is what I get if I scroll all the way down.*

Maybe I'm just salty and sensitive, but sure -- even if the bulk toggles were at the bottom and we want to serve fine-tuned items first, why are the disclosures not provided next to those toggles? Particularly those that say it takes 60 days for individual preferences to be honored -- why is that information divorced from the rest? Perhaps the end user doesn't find this information useful or thinks it's truly fine-print content; all extra stuff that they don't have time for. And that's more than fair; users want value fast and don't have as much time as me, someone researching this stuff, to read every single piece of tiny-font gray text. 

However, I've learned to expect bulk actions to be available at the top of interfaces; in spreadsheets, does anyone ever do anything to a column by using controls at... the bottom of a column? No. When you want to do anything en masse in other table-oriented or nested designs, is the bulk option at the bottom?? Most likely not! Think of menus and expand all/collapse all options; those are usually prominently or at least logically displayed near the _top_ of the design for whatever needs to be managed in bulk. 

In my opinion, there are a number of things wrong here.
* The "all" options are divorced from the actual items they manage and are presented as a distinctly separate option
* The bulk toggles aren't visible anywhere on the first screen that will show for most users
* The bulk toggles require scrolling
* The disclosures on processing time for individual toggles are not near the individual toggles
(And, of course, while my screenshots show everything as opted-out, they were opted-in by default when I first opened the link). 

These designs obfuscate the truth of what the user's options are and don't present options equivalently in value, nor transparently (with all the hiding). Users are forced to take on the labor of scrolling, clicking, reading, toggling, and waiting in order to avoid an interaction that is defaulted in the best interests of Xfinity. Xfinity deploys this at scale; it's trivial for them to send emails to anyone who goes through the effort of registering with them. Users cannot operate at-scale. You tell me who loses out with shady practices like this. 


### On CAN-SPAM Compliance
Earlier I asked whether having all the frontend discosures and buttons indicated CAN-SPAM compliance, and no, they do not for Xfinity's case (as far as I can tell with a cursory search through applicable regs). It's bad enough that compliance is a losing battle with a lot of labor costs attached and it's easy to pass an audit at one point in time and fall back on non-compliance until the next period of scrutiny!

The [FTC's CAN-SPAM Compliance Guide for Businesses](https://www.ftc.gov/business-guidance/resources/can-spam-act-compliance-guide-business) states that orgs should:
> **Honor opt-out requests promptly.** Any opt-out mechanism you offer must be able to process opt-out requests for at least 30 days after you send your message. You must honor a recipient’s opt-out request within 10 business days. You can’t charge a fee, require the recipient to give you any personally identifying information beyond an email address, or make the recipient take any step other than sending a reply email or visiting a single page on an Internet website as a condition for honoring an opt-out request. Once people have told you they don’t want to receive more messages from you, you can’t sell or transfer their email addresses, even in the form of a mailing list. The only exception is that you may transfer the addresses to a company you’ve hired to help you comply with the CAN-SPAM Act.

Correct me if I'm wrong, but last I checked, 60 != 10. Sounds great, right? Clearly the emails I've been getting, or even the disclosures Xfinity provides, should get dinged as non-compliant, right? The official opt-out prohibitions for all emails are for charging fees or requiring information for opting out, in Section 316.5 -- subrules then link to 15 U.S.C. 7704(a)(3)(B) and (a)(4) which mandate that 10-day rule. With a quick read, I'm not entirely sure when that 10 days kicks in, but it sounds to me that it kicks in within 10 days of _receipt_ of the opt-out _request_, which Xfinity is now at least 42 days behind on for my case. 

Well, great -- if they're non-compliant, now what? Personally, I don't know where to go to do anything about this and while this wasn't a waste of _my_ time (this is great fodder for future research), this is certainly frickin' annoying and (hopefully, if I read things correctly) illegal. 

The FAQ on that [Compliance Guide](https://www.ftc.gov/business-guidance/resources/can-spam-act-compliance-guide-business) states that
> \[each\] separate email in violation of the law is subject to penalties of up to $46,517, and more than one person may be held responsible for violations
... and boy, would I love to see that actually happen. 

But for now... I'll be happy with just a full stop on those advertising emails, please. And we'll see if that just-in-case 60-day thing gets honored by next week. 

-----

Oh, and one more thing; in the inbox screenshot above, I followed the unsubscribe link on the 4/21 email, which led me to a defunct URL... which proooobably bricks 15 U.S.C. 7704(a)(3)(B) and the 'functioning' bit of 15 U.S.C. 7704(a)(3)(A). Oh, and 15 U.S.C. 7704(a)(3)(A)(ii), since I checked that unsubscribe link well within 30 days of initial receipt of that 4/21 email. 

<img src="https://johannagunawan.com/assets/img/blog/2022-04-27-xfinity-unsub-brickedpage.png" width="750">
*The 4/21 email's unsubscribe link doesn't... even... work.*

I took a look at the URLs for both and found that the parameter strings for the 4/21 email does not match those from the prior two emails. The strings for the 3/30 and 3/27 email match more chars except the last 20 or so, but still lead to the usual site. The 4/21 email's link, however, either poorly formats the params based on my inbox/email metadata, or has other bugs, and stops matching the params string for the last 163 chars. I haven't reproduced the links for security reasons, but I've got record of them to fuel my own rage.