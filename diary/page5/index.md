[2021-04-25](/diary/2021/04/25.md)

Well, it's been a while.

The Punk Collective met last Wednesday in the city. Burgers for lunch, following an impromtu tour of a nearby co-working space. Really conveniently located; accessible directly from the main underground train station, and just a 10-minute journey from my local train station. Seriously considering a membership; it's around $150/mo for five days access per month, which is around what I think I need (basically get out of the house and meet up with other solo developers once a week or so).

Apart from that, have been working on Blattix! I've added walls, collisions, shooting, sound effects and music (purchasing ten punk rock tracks for unrestricted commercial use for $99). Controls feel tight, and it's fast.

![SSS1](/diary/assets/sss1.png)

Next steps are to get a simple game loop happening (I'll just make Asteroids for now) and get builds shipped out to the other punks. This will mark the end of the first month of development, and we're limiting ourselves to just three months. In the second month, I will focus on refactoring and fleshing out the gameplay, adding waves of different enemy types, progression through levels, boss battles and so on. The final month will be bugfixing, polish and optimisation.

Remember that I'm trying to limit myself to spending just a third of my time on this particular project, so next month I plan to make some room to continue work on Gumshoe and HackTile. Busy times.

Unfortunately we've gone into a snap lockdown due to some community transmission in Perth. I'm focusing on a three-day gamejam to distract me from those concerns, and things will hopefully be back to normal soon...

[2021-04-02](/diary/2021/04/02.md)

Sidetracked by our Punk Collective commitment to build a game each in the next quarter. The other three punks have been super productive with their games, and so I spend the week working on something myself... Blattix!

![Blattix](/diary/assets/blattix.png)

This will be a retro-style shooter with multiple waves of enemies, going for high replayability rather than depth of content. I've drawn inspiration from [Encounter](https://youtu.be/4CHN-usjFfE?t=12), [Cosmic Causeway](https://youtu.be/i2SvzHY6JhY?t=1), [BallBlazer](https://youtu.be/ISXUs6kYS2Q?t=24) and [Vaxine](https://youtu.be/cT4fGokPVJ4?t=166).

It's been an excuse to learn some shader programming, and to brush up on my linear algebra. I'm not using a 3D game engine at all, it's just rendering sprites and doing a bit of tricky jiggery-pokery. Next I will move on to building a simple physics engine, which will allow collisions between objects, enabling some shoot-em-up gameplay.

Lots of fun!

[2021-03-25](/diary/2021/03/25.md)

Third Punk Collective meetup yesterday. Everyone seemed reluctant to meet and had various excuses, but in the end it all came together and we had the best meeting so far. We were all on the same page and spoke about creating and publishing one small game each in the latter half of the year, mostly to learn the ropes end-to-end and to attempt to build an audience. Looking forward to that!

The GumShoe refactoring is progressing nicely, and I can now see the light at the end of the tunnel. The game is still not quite there yet; the refactored version is janky and missing features when compared to the demo that I hacked together last month, but the code is much nicer to work with and to build upon, and it will make it easy for me to experiment with realtime client/server updates, and perhaps with multiplayer.

I'm really looking forward to getting all that done and dusted so I can get back to HackTile, which I think has great potential. Need more time in the day!

[2021-03-11](/diary/2021/03/11.md)

I wrote a [blog post](https://medium.com/the-magic-pantry/the-case-of-the-fake-database-7bde487213a3) about RnDB _and_ recorded a video walkthough (which is linked to from the post), and had a decent response on Reddit (prompting me to add a few new features, particularly the ability to load and save mutations). Very nice to complete something, ship it and get feedback from the community in such a short window of time. And I can now cross RnDB off the list of project ideas that constantly nag at me in the back of my mind.

I discovered [Standard Ruby](https://blog.testdouble.com/posts/2021-03-04-announcing-standard-ruby-1.0/) and spent a bit of time making my existing project repositories compliant, but this in part was to distract myself from GumShoe refactoring, which is progressing slowly. It dawned on me that the process isn't so much one of coding but of re-arranging things in your head. After many days of thinking and a few false starts I now have a rough architecture that makes sense, and I'm working to finish the refactoring and have a demo of the back-end integration up-and-running by early next week.

This will coincide with the end of [The 7DRL Challenge](https://7drl.com/), which some of the other Punks are participating in. Beetlefeet is building an awesome golf rpg, while Maxxor is making an apocalyptic wasteland with dynamic lighting effects. At our second coffee shop meetup yesterday they showed great progress. Chr15m started strong but bowed out after his Office Brawl simulator failed to light a spark, which is precisely the right thing to do. Follow the passion and fail early. Great to see!

[2021-02-25](/diary/2021/02/25.md)

After a lot of focused work on Gumshoe, I reached a milestone that allowed me to put together a simple, complete game, which is currently playable online. It's fun, and easy for others to pick up and try. But all this rushing meant that some refactoring and tidying up was in order, and, instead of doing that, I decided to descend the procedural generation rabbit-hole.

I've finally come up for air, releasing [RnDB](https://github.com/kranzky/rndb) into the public domain as evidence that I was actually doing something. Over the coming weekend I'll finish that off, perhaps recording an explanatory video.

It's an itch I've been longing to scratch for a while, having first has the idea while working on LA Noire at Team Bondi in 2005. So great to get it done and shipped in just a week or so of intensive work.

Beetlefeet, Maxxor, Chr15m and I have established "The Punk Collective", which is a support group of sorts for solo developers, and our first gathering at a coffee shop mid-week was super productive and inspiring. The aim between now at the next gathering will be to knock off all of the Gumshoe overhaul work, together with back-end integration. Beyond that, I'd love to get back to HackTile, but who knows really?

We also bumped into Shrydar during our meeting, who was grabbing a fluorescent green milkshake, and brought us the sad news that the coffee shop will soon be closing down, which will be the end of an era. We briefly discussed leasing some office space somewhere, as I'd enthused everyone about the Loonshots Nursery idea. We'll see where that goes.

Shrydar is still coding c64 demos, which is totally awesome to see.

[2021-02-09](/diary/2021/02/09.md)

Have spent the last week or so working on Gumshoe, a GGJ project that I started with Beetlefeet, using the lets-punk project template. Here's a screenshot.

![Gumshoe](/diary/assets/gumshoe.png)

It's destined to be a text-based roguelike detective game. But it's also a crash course in using Quasar and Vue, and I am back-porting all of the improvements I make to the lets-punk template, and then porting them over to hacktile.

I have established a very comformatble hack-refactor-polish loop, whereby I quickly implement a new feature, then refactor the code to settle it down (as it often means code needs to be dry'ed up or improved elsewhere), and I then polish the UI, adding transitions and animations and making sure it's responsive and works across all devices.

Have it working as a PWA on Android and iOS, with update notifications too. It's feeling very slick. We've also exited lockdown and kids are back at school, so feeling even more productive.

Aim is to ship Gumshoe to get feeback from friends towards the end of this month, and then transition back to hacktile for most of my time.

[2021-02-01](/diary/2021/02/01.md)

Over the last week I did some tidying-up work on the Hacktile project, and back-ported some changes to the LetsPunk template. I then used that template to start a new project, Gumshoe, for the GGJ. It's a procedurally-generated detective game, but it is also an excuse for me to learn more about Quasar and Vue, and practise UI coding, so it will benefit other projects too.

Demo here: [gumshoe.kranzky.com](https://gumshoe.kranzky.com)

I will continue working on this in tandem with HackTile, switching between the two projects to maintain enthusiasm, and back-porting changes to the core framework that I make as I continue to learn.

In other news, we are in hard lockdown for five days. The kids should have started school today, but summer holidays have been extended for a week.

[Previous](/diary/page4) Page: 5 of 26 [Next](/diary/page6)