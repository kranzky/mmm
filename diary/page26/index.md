[2018-05-26](/diary/2018/05/26.md)

Eliza's 12th birthday. Kids up early. Presents and breakfast, then took the kids to Garden City. Jack had a haircut, Eliza bought herself a Pokemon game. Back to prepare lunch; roast lamb with all the trimmings for 17 of us (both sides of the family). Played the C64 and the SNES with my brothers. Afternoon spent cleaning up and making lamb and barley soup for dinner. Played Letter Tycoon with the kids before they went to bed. Far too tired to work on HackTile; will watch an episode of The West Wing and crash.

[2018-05-25](/diary/2018/05/25.md)

Very tired today. Slept little partly because I broke my own rules and stayed up far too late last night (watching The West Wing, listening to The West Wing Weekly, then listening to music, drinking whiskey, reading), and partly because I couldn't stop coughing once I'd gone to bed.

Storm overnight. Heavy rain and strong winds. Feels like winter! Lots of shopping today for Eliza's birthday lunch tomorrow. Wrapped her presents and made a photo collage of her last 11 birthdays, and the day she was born.

Implemented a camera system for HackTile, allowing me to pan and zoom around the playfield using the XBox controller. Pretty neat. Oh, I promised a screenshot:

![Camera Experiments](/diary/assets/camera.png)

Yup, it's still only Conway's Life. The red lines show the border between the 4k texture that represents the entire world. It's being tiled because the camera is zoomed way, way out (until each 16x16 pixel entity occupies only a single pixel on screen). We can zoom way, way in, too, up to 128 times:

![Camera Zoom](/diary/assets/zoomed.png)

Mum and Dad over for Friday night dinner. Finlay for a sleepover. Watched Wallace and Gromit with popcorn after a stodgy meal of shepherd's pie, potato gratin, lasagna and apple tart. Heaven.

[2018-05-24](/diary/2018/05/24.md)

Busy day at work... knocked off a few major tasks, and followed up after a late-night meeting yesterday with a development team in Chicago.

Battening down the hatches this afternoon in preparation for an overnight storm. Winter is coming...

HackTile progress. Added vsync to the render loop, and changed the update function of the engine to allow the CA to update just 10 times per second (before that, after implementing empty space instead of requiring entities everywhere, it got up to 160 updates per second). Next on the list is to scroll and zoom the viewport.

Eliza had Cindy K over after school to do some baking. Jack had an asthma attack at school after doing cross-country training. And I headed off to the doctor's to get some steroids to fight my own asthma (a side-effect of the cold).

Electrician over to fix the power points in Eliza's room. Dzung very busy at work; she had a late brunch with April and Mary and then working all day. I made leftover curry with roti and rice for dinner. Calling it a night early... plan to veg and get some rest.

[2018-05-23](/diary/2018/05/23.md)

Jack headed off to a whole-day excursion to SciTech. Eliza in early for Japanese before school begins. Me doing some shallow work in my PJs while Dzung drives them in.

Have a work meeting scheduled for late tonight, and had trouble this morning getting motivated to work my regular job (due to politics mostly, we focus on trivialities which don't serve to push us towards our goal). So, in penance for skipping out on _HackTile_ yesterday, I spent some time working on it during the day. Some progress made; refactored so that the engine creates and destroys entities in the game, which the game renders. Achieved 55fps with 65536 entities running Conway's Life. A screenshot tomorrow, perhaps.

Lunch at a Hawkers place for Laksa, after watching Adam Liaw make a fantastic version of that dish on YouTube last night.

Health much the same as yesterday. Cleaned up garden. Salmon dish for dinner.

[2018-05-22](/diary/2018/05/22.md)

Scheduled the day again. Realised I can break it into 4 blocks:

- 7am - 9am: Shallow work (active 1 hour)
- 9am - 3pm: Deep work (active 4 hours)
- 3pm - 9pm: Shallow work (active 2 hours)
- 9pm - 11pm: Deep work (active 2 hours)

By shallow work, I mean things that would take me a few weeks to train somebody else to do. By deep work, I mean things that require intense concentration, and which leverage the domain knowledge and engineering skills that I've built up over the last three decades. By active, I mean sitting at my desk doing real work, and not just pretending to be busy. In breaks I can still passively work, by answering emails and things like that, but I may be doing that on my phone while I'm distracted with something else.

This makes sense to me. It's hard to do more than six hours of active, deep work in a single day. It can be mentally exhausting. Most "knowledge workers" in a traditional open-plan office would struggle to achieve half of that. But that's where the value is.

I like that rough schedule. It gives me time to work my main job, and time to make progress on hobby projects.

Speaking of which, didn't work on _HackTile_ at all today, even though I'd planned to. Got delayed reading _The Queen of Sorcery_ to Eliza and cleaning up the kitchen, then listened to two episodes of _The West Wing Weekly_. It was too late after all that to begin working on something.

Kids had their flu shot today. Picked up Eliza from string orchestra practice early. Jack being very silly (annoyingly so) all afternoon. He's developed a habit of lying for fun. Must change that. Dzung made pork ribs for dinner. I'm doing OK; still 75% health after recovering from this cold.

[2018-05-21](/diary/2018/05/21.md)

Watching S02E01 of Legion. Amazing sound design.

Refactoring some of the _HackTile_ code. Pretty easy to get things up and running with SDL2, and I have a basic CA working (Conway, of course). Updating 50k cells at 50Hz minimum. I remember why C is so much fun!

Still unwell. Made lamb rogan josh for dinner... the kids can handle curry these days. First time making Indian for the whole family though. Eliza had Quiz Club after school. Jack played the trumpet during a music incursion.

Deep work is paying off. Scheduled each hour of the day. Doesn't take much effort to do, and I found I could focus and commit to a particular task more easily. May it continue!

[2018-05-20](/diary/2018/05/20.md)

I've decided to start keeping a diary again.

I'm 46-years-old and working from home for a US-based startup. My kids are 11 and 8, and doing well at school. My wife works from home once or twice a week, which allows us to have lunch together.

It's nice, but I want more. I want to be creative, and do good work.

I also want to generate a passive income.

I have a few project ideas kicking around:

- Jack and I are working on a password manager "for your mum".
- Jack, Rob and I still occasionally post to our "Link a Day" Slack channel.
- I've started toying around with SDL2 and vanilla C again.

Yes, C. It's quite refreshing, and I think decades of experience with higher-level languages means the C code I write nowadays has matured without me knowing about it.

Anyway, I plan to resurrect the _HackTile_ project. Hopefully this diary will help me keep track of that. But I get easily distracted from side projects.

I'll be trying to apply the principles of "deep work". I'll schedule daily blocks of time to work on one of the aforementioned projects, and I'll track my progress by writing it down here. I want to keep at it for at least 100 days, like I did with the 7-minute workout. That'll help to make it a habit.

But I'm still recovering from a severe head cold. It's a beautiful Autumn day, and we had a lunch of _banh-mi-tet_ at the park in East Perth, but back home now with the kids (looking after Lilian, Lachlan and Yoshi because their parents are at the footy).

Future posts will be shorter. I just want to capture the essence of each day.

Onward!

[Previous](/diary/page25) Page: 26 of 26Next