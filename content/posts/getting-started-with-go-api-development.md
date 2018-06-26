---
title: "Getting Started With Go Api Development"
date: 2018-06-26T13:41:45-05:00
---

## Prepare to enter a restart loop ##

I've been poking at using go for a side project for about a month now, and I don't have much to show for it.

Other than a vague feeling that >1000 other devs have recently made this same troublesome, looping sojourn, I'm left with not very much concrete progress.

Two images spring to my mind:

1.  Back in like 1996, I had a sweet geocities webpage where I fiddled around learning html.  I had found an animated gif of a guy drawing furiously on a drafting table, then he'd crumple it up and discard it over his shoulder, on loop.  Even though google image search now fails me, I can still see this gif vividly 22 years later, and feel his pain anew.
    {{< figure src="/madhack.gif" >}}

2.  The Wheel of Time's Aes Sedai serpent-eating-itself ring. (I just finished book 4, finally... only 10 more to go...)

## The best framework is no framework.  Maybe. ##

So if one thing is perfectly clear to me now, its that there is no love for the word 'framework' in go.  If you're aiming to make a reusable project ***DONT CALL IT A FRAMEWORK***, or you will have doomed your project to complete failure.  'Toolset' might be ok?  I haven't really figured out why, but my guess is that once something is big enough to be called a 'framework', it is so full of opinions and possible bloat that no sweet-spot community forms around it.  It ends up inheriting so much of the dev who created it, and contains tools suitable to whatever their usecase, that it alienates all others.  ??

My journey has been like (I assume) the other devs before; I look for something opinionated (like Spring for Java, or Django for Python), find a few things, but the trail always sort of fades out before full fruition.

I basically (think) I want:

* a request router - [gorilla/mux](https://github.com/gorilla/mux) seems to be fine for me, but theres some good examples out there using [echo](https://echo.labstack.com/) as well
* a testable project structure - I'm pretty new to TDD, but this seems too important to not be a thing
* some auth middleware - some sort of basic-auth login with [securecookies](https://github.com/gorilla/securecookie) is probably enough to get me started?  but [go-jwt](https://github.com/dgrijalva/jwt-go) led me down a few other paths as well...
* something that takes repitition out of my database operations... marshalling json->struct->db... I'm not sure if this is actually an 'orm', but I've spent some time with [go-pg](https://github.com/go-pg/pg), [sqlx](https://github.com/jmoiron/sqlx), [gorm](https://github.com/jinzhu/gorm)...
* oh, should I mock my database?  not sure!  lets spend some time with [testfixtures](https://github.com/go-testfixtures/testfixtures) instead

The problem seems to me that alot of these things are semi related, and I haven't found an example project that nails them all.

Projects / blogs that seem to 'feel my pain', but still leave me starting over:

* [a great tutorial](https://semaphoreci.com/community/tutorials/building-and-testing-a-rest-api-in-go-with-gorilla-mux-and-postgresql) - Shows a way to structure your project for writing tests, A++ learned a lot from this.  However, no database orm, and good lord I'm not sure I'm up for all the repetition that'd go into my project without one.
* [gobuffalo](https://gobuffalo.io/en) - I really wanted this to be the answer so I could break out of the loop; Mark's presentation video on the homepage spoke to me as if it felt my pain.   It might still be an answer, I dunno.  Indecision overwhelms.
* [go-mux-jwt-boilerplate](https://github.com/hellojebus/go-mux-jwt-boilerplate) - I feel like this guy is me in 1 month.  He's made some progress, finally, and has a decent project structure.  But he has no tests, which seems to be like 50% of the challenge.
* gorsk ([blog](https://www.ribice.ba/golang-web-frameworks/) / [repo](https://github.com/ribice/gorsk)) - This is probably what a legit experienced developer does.  He's taken his time, done a bunch of research, swapped things around, formed his own opinions, and now probably has something he likes.  The problem is its now 20x more sophisticated/complex than what I'm looking to start with.  And so the wheel continues to spin...

## So where am I now? ##

A big part of my problem is wanting to run before I can walk, or maybe even before knowing what walking is.  Another part of the problem is when you're copying nuggets from blogs and other project readmes, you lose sight of the fact that this is **YOUR DEVELOPMENT PROBLEM TO SOLVE**; you lack ownership because you're not really developing.  This is a problem for me because I tend to go into analysis paralysis ("this solution seems like too many lines / files / functions / complex-interface-stuff-i-dont-understand-yet, lets sit and stare at 12 others before starting over yet again in some slightly different way").

So.  Time to focus on the basics of the language, learn, start small, and stick with it.  I may eventually need 12 other projects all tied together neatly, but lets start with the basics.
