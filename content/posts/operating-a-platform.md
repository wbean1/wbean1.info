---
title: "Operating a Platform"
date: 2018-06-06T19:11:18-05:00
draft: true
---

# So you want to run a platform...

Firstly, are you sure?

The as-a-service revolution is well underway, as [this great article from Luke Kanies](https://medium.com/@lkanies/the-binary-future-of-software-companies-36851123ddeb) spells out.  See also the momentous, if not dated, [PaaS for Realists](http://blog.lusis.org/blog/2014/06/14/paas-for-realists/).  Running your own anything anymore seems to be for the birds.

{{< figure src="/bird-shit-in-hair.jpg" >}}

But ok.  You have your job cut out for you.

What are some of the requirements for running this thing you're endevouring to deliver?

```
0. **Uptime** equal-to-or-greater-than **100%**.
```    
Ok.  This _might_ be harder than you thought.
    
Let me spell out some of the things I've gleaned from actually endevouring on this in a large enterprise.
   
1. **Frequent Updates** - 
    
    Systems have flaws.  People have flaws.  Shit changes.  You need to be able to deliver these changes reliably into your platform.  You need a CI/CD system.  There are many; learn a few, evaluate, implement, refine.  Get comfortable changing your platform while its running _before_ you start selling it.  The more frequently you excersize a process, the less error-prone it will become.
    
2. **Monitor More Everyday** -
    
    Systems are living, breathing, entities.  Shit will happen, and you will be asked to explain why.  And expected to be able to figure out why.  And expected to make sure that thing either **NEVER HAPPENS AGAIN**, or can be squashed with automation before there are any effects.  System metrics, logs, events, alerts, data data data.  Make it a point to know what is going on inside your platform. 
    
3. **Did I Mention To Test?** -
    
    Don't be the guy that wants to yolo things into prod.  Have tests.  Run them.  Have a peer.  Review each other's work.  Take turns shooting holes into PRs, Theories, and Tasks.  Don't let each other take shortcuts.  _RUN SYSTEM TESTS CONSTANTLY_, even on your test systems while you're trying out something new.  Literally don't do _ANYTHING_ in prod that you're still uncertain of from test.
    
4. **Plug Into the Community** -
    
    Unless you're a super masochist, your platform is probably one that others are also operating.  Meet those people.  They probably are alive in Slack.  Or at super hip conferences.  Help other people, and contribute.
    
5. **Have An Opinion** -
    
    _But keep an open mind_.  You are probably paid because you are good at analyzing a situation.  Systems need [guard rails](https://12factor.net/), and [guardians](https://www.imdb.com/title/tt2015381/mediaviewer/rm1108790784).  Have a holistic and realistic view of your system.  It probably won't [slice your bread or make you coffee](https://www.ietf.org/rfc/rfc2324.txt) on day 1. 
    
6. **Keep The Excitement Alive** -
    
    Not every day will be your best day.  Your system won't be perfect.  But it might still be pretty damn good.  And if you're around making it better, there is  still hope.
