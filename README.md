
# Hello there!

I am Ingwie. Since I am not too keen on sharing my real name online, I decided to use the nickname given to me when I was in my second year of school and added the species of my previous furry persona; a phoenix. Hence, **Ingwie Phoenix**. :)

## What I do...

Mostly just dumb sh't! I have ideas, try to implement them, run into a wall and end up abandoning them. I am the kind of guy that just tries things out a lot - and if it leads nowhere, I just let it go and come back at some other time to possibly continue working on it. Not the most persistent guy, you think? Yeah, kind of true. But I have no real direction right now, no real "big project" I want to finish ASAP, just a bunch of ideas, concepts and started code.

## What I am (kinda) working on...

- **A build tool**. I don't like CMake's syntax, believe it could be made sleeker, slimmer, smaller and yet include more features. I want to implement it in the [V programming language](https://github.com/vlang/v). The old name was `IceTea` - but I am starting to like the idea of calling it `Maid` instead.
  * It's supposed to allow everyone to get started with build automation. A one-liner should be enough to build a folder filled with C files into an executable, and a second should be enough to add a dependency.
  * It's supposed to be cross-platform. V compiles to C, and due to the [way V picks files to compile](https://github.com/vlang/v/blob/master/vlib/v/pref/should_compile.v), it's totally possible to write near abstractionless code! No structs containing callbacks, just plain implementation picking at compile-time. This should make for really great cross-platform portability.
  * It's supposed to have more than just one way of usage. My primary goal is to use [JerryScript](https://github.com/jerryscript-project/jerryscript) to provide a JS interface to write build descriptions in. But obviously, you could just write it in V directly - so that is what I am also aiming for. Use JS for a high level, great looking API but V for a more low-level approach, allowing deeper interactions with the APIs.
  * It's supposed to integrate. Although I plan on implementing a command scheduler and executor, it doesn't hurt to allow interfacing with other tools. For instance: Using a preprocessor like [xPP](https://github.com/symisc/xPP), it'd be somewhat possible to process M4 - or, just use a M4 parser directly. And, CMake even has a [server protocol](https://cmake.org/cmake/help/v3.7/manual/cmake-server.7.html) that would allow for some neat integrations. That way, dependencies could retain their original buildsystem and would only use a description file to tell the system that, hey, use CMake here and pass those information to other targets so they know a little about this.
- **An Electron alternative**. You might have noticed that I own the [appJS](https://github.com/appjs) org? Back, WAY before Electron, effords were made - not by me, mind you - to utilize CEF (Chromeium Embedded Framework) and a node-like reimplementation ontop of it to create what we know today as Electron. A while after appJS, Adobe Brackets used a similar approach, using a NodeJS process launched alongside and an RPC interface to make them talk. When Github Atom launched, the first version of Electron was shown to the world. This is all great and what not - but it's quite a problem for specifically older hardware. For instance, I run a MacBook A1342 as my backup maschine. More than two Electron apps, and the poor thing just melts on the spot... Plus, most of those apps completely ignore accessibility. I believe that there is something better that could be made that would incooperate native accessibility technology and be way smaller.
  * To make an Electron competitor, it needs to support HTML, JS and CSS.
  * There is a project called [Netsurf](https://www.netsurf-browser.org/) whose source code holds an amazing amount of useful tools and libraries. Using parts of that should give a great basis.
  * Now, just displaying web-ish stuff is not what Electron is ment to do; it's ment to display apps, right? So instead of rendering a "website", I am intending to utilize [LVGL](https://lvgl.io) to render widgets/components.
  * Using the excellent [SDL](https://www.libsdl.org/) library, there is already a great deal of cross-platform compatibility.
  * Ultimatively, I want to have the framework itself usurp SDL and utilize V's abstraction-less coding instead to slim down the compiled code and improve readability and API design.
  * The old, initial title for the project was `Phoenix Engine`. Now, I am leaning more towards `Vision`. My *vision* of modern, cross-platform app development. Resource-saving, platform-respecting and non-excluding apps that run basically anywhere. And yes, accessibility is very important to me as a visually impaired people, having grown up inbetween people with several dozens of impairments, that all just want to use a computer but often get denied by new-fangled, fancy-pants but ultimatively inaccessible apps. Just look at the state of accessibility on Linux. It's... tough...
- **Porting V to new places**. Since V is a language I like quite a lot, I'd love to see it in more places. My personal, most favorite target that I want to port V to, is the GameBoy and GameBoy Color. GameBoy Advance is already *somewhat* possible since V has an ARM output option, but the old GB/C would be a fun project to work on, learning how to write an assembler and go allt he way from V to C to ASM to binary! But... I, alone, can only do so much ^^;
- **A trading card game simulator**. Way, way way way back I discovered trading card games like [Cardfight!! Vanguard](https://en.cf-vanguard.com/) and [WIXOSS](https://wixoss.fandom.com/wiki/WIXOSS). But, due to the inpopularity of TCGs - aside from Yu-Gi-Oh! and Magic: The Gathering - here in Germany, there is just no way I could play it. At all. And, the pandemic made this *even harder*. Hence, I would love to implement both of those games eventually - but, why not start at the basis?
  * I want to design an interface with the idea of RetroArch: One end designs the game, the other end designs the UI.
  * As for the "backend", I want to lean heavily on [libocgcore](https://github.com/Fluorohydride/ygopro-core). It's battletested, stable and the API looks good. Although it's in C++, porting the basic ideas to V should be no problem. Even if V is missing "true OOP", there is still enough of it (struct methods, interfaces) that it will do just fine!

Noticed something? All those projects actually build up on one another. It's been a dream of mine to write my own *actual* game. Not those practice games you write in programming class - no. I mean an actual, real-deal game. I won't ever get close to the game that inspired me to write my own, [Drakengard](https://en.wikipedia.org/wiki/Drakengard), simply due to my visual impairment, but still. I want to get there some day! ^_^

## Visual impairment...?

I mentioned it a few times, so let me outline it:
- I have a visus of about 16% on my left, and .3% on my right (which is only an estimate due to just how bad it actually is)
- My field of vision is miniscule. Like, really, really tiny. Ever tried peeping through one of those classic keyholes you could actually peep through? Yup, that's my FoV. And, only on my left eye. My right eye is even worse.
- I am reliant on screen magnification and big screens. Both are easy to get by (except on Linux **coughcough**) and that really is all I need. Well, and a keyboard that doesn't eat my keystrokes...

## Wanna chat?

If you would love to talk, feel free to ping me. I'm not doing much, so go ahead! o.o

- **Discord:** `IngwiePhoenix#6637`
- **Twitter:** [@IngwiePhoenix](https://twitter.com/IngwiePhoenix)
- **Matrix:** `ingwiephoenix:ingwie.io`
- **Telegram:** `@IngwiePhoenix`
