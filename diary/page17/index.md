[2018-07-28](/diary/2018/07/28.md)

No HackTile. Kids to karate with Dzung. I read "Kavalier and Clay" for a while, after finishing chores, and then got to work unblocking the drain in my bathroom. That worked, so checked other drains, and Jack's needed some love too. Worked on that, but accidentally pressed down the plug so it couldn't be removed. Ended up working for an hour, had to take everything apart and reassemble, then repeat when my first attempt leaked. Next time I'll call a guy.

Out in the afternoon shopping for stools. Found a couple we like; Hudson's mum was the salesperson and let us bring them home to try out. They're not high enough. Cooked dinner with Dzung; pork ribs, beans, coleslaw. Then played some VR together before putting the kids to bed. Ended the night watching "John Wick 2" with Dzung, an abysmal film.

[2018-07-27](/diary/2018/07/27.md)

Easy morning. Decided I'd take my foot off the accelerator at work until design and requirements sort themselves out. Don't want to rework any of the backend. Planned an easy day of fixing a few issues and getting some chores done: banking, cleaning, shopping and a blood donation. But they cajoled me to donate platelets instead of blood—I was reticent to do so due to my bad experience last year—but they were very kind and careful and it all went well. One of the young nurses flirted with me, saying my arms were lovely and warm and that I would "be a girl's best friend on a cold night". Flattering but awkward; this all in front of a room of other donors. Didn't know what to say. Ended up taking a large chunk out of my day. Even worse, returned home dead tired, a combination I think of deciding to work less intensely and the loss of blood. Mooching around in the afternoon; mum and dad over with shepherd's pie for dinner. Yum. Too worn out in the evening to code; vegged out in front of the TV before having an early night.

[2018-07-26](/diary/2018/07/26.md)

Very busy at work, but blindsided by a design coming out of nowhere, with it's own user stories, in no way following the documented spec. Worked furiously all day, from 7:30 to 17:00, with nary a break. Exhausted, cooked the salmon dish for the kids while Dzung took them to piano lessons. Philae arrived after dinner to mind the kids while Dzung and I went to "The White Album Concert". Third time we've been; other shows were in 2009 and 2014. Absolutely fantastic. Home at 23:00 to crash on the sofa and watch the last episode of "Sense 8". Too tired to finish it, I crawled to bed. Obviously no HackTile.

[2018-07-25](/diary/2018/07/25.md)

No HackTile. Extremely busy at work. Frantic. Dzung not feeling very well. Massive downpour at school pick-up time, trying to contact Eliza to tell her to stay undercover at the school, but that only ended up delaying me in traffic while she walked to the usual meeting spot in the park and got soaked. She cooked dinner, following a recipe from "You Plate It", using ingredients we bought ourselves. Finished the night watching a couple of episodes of "Handmaid's Tale".

[2018-07-24](/diary/2018/07/24.md)

Long, busy day. Heaps to do at work. Skipped lunch with Wil, and cancelled meeting with Will tomorrow. Eliza off early due to parent-teacher meetings; she had a ball visiting her old primary school with her friends. Walked home with both kids, just like old times (sob).

Dzung out for Chang's birthday, after rushing home to meet with Eliza's maths teacher. She's a great mum. I took the kids to the shops to buy ingredients for Eliza to make tomorrow night's dinner. Then picked up a huge feast of fish and chips, which we ate while watching the beginning of "Spiderman: Homecoming".

Still working into the evening. Will watch an episode of Handmaid soon, then crash. No time to even think about HackTile.

[2018-07-23](/diary/2018/07/23.md)

Got some chores done once kids were at school. Lots of work-related chatter. Did three or four hours over the weekend so took it easy. Feeling less sore today, so did three circuits of the 7-minute workout while listening to a podcast. Eggs, toast and coffee for lunch while watching an episode of The West Wing (now that I've caught up on the podcasts I need to watch a few episodes again).

Thinking about rules. Lots of thought experiments, like having magnets that repell a ball. What happens when a ball-magnet pair face each other with a gap in-between? There are three possibilities.

- One ball wins, which blocks the other ball from moving. This isn't ideal, because it breaks the assumption that all rules are processed in parallel. Why would one win?
- Neither ball wins (we detect there is a conflict, which causes both rules to fail). This isn't ideal, because there's an obvious gap for the balls to move into.
- Both rules succeed, and the two balls begin moving towards each other. But then both rules are reverted (because of the conflict) and they move back to their original position.

I like this last solution, as it yields the intuitively correct behaviour; the balls will wobble back-and-forth. The magnets have an obvious and consistent effect on the world, and the world rule of one entity per cell is visually not violated. It implies rules having multiple states, and the engine updating between rule transitions. Things like sound effects could be triggered by the rule beginning to execute, by the rule succeeding, or by the rule being rolled back. That should give a lot of expressiveness to the engine.

Another thought experiment is an NPC that has four rules, each telling it to move in a different direction. In this case, only one rule can succeed, as they are all attempting to move the entity. Essentially the movement command requires exclusive access to the resource. It's fairest to select one rule to win at random, meaning NPCs will get random (brownian) movement for free. Nice.

Apart from movement, there aren't too many commands that require exclusive access to a resource. Really just movement and mutating a register.

Final thought experiment is back to the magnet-ball rule, where the balls are adjacent, with another rule that adjacent balls de-spawn (in a fiery explosion), with magnets strategically positioned to push the balls apart. What should happen here?

- The rule to explode the balls beats the rule to move the balls, and so they explode.
- The rule to move the balls beats the rule to explode the balls. and so they move.
- Both rules fire, so the balls explode while they're moving.

Again, this last case seems intuitively correct. The rule to explode the ball simply de-spawns both balls (which plays an explosion animation), and triggers an explosion sound effect. The rules to move the balls still fires, but the entity engine can handle moving an entity while it's de-spawning, so there's no conflict to rollback.

All of this comes naturally when we think of the 3x3 grid as providing context to decide if a rule should fire, and the rule itself then issuing a series of commands (such as move entity and so on), rather than the rule mutating the 3x3 grid (which is what the user may see when editing rules, but not what the engine works with when executing rules).

Anyway, that's a bit of a thesis. Hopefully things will solidify somewhat over the next day or two so I can begin coding this up.

Jack had school photos today. I cooked bolognaise for dinner. Full from overeating! Dzung and Jack watched Australian Ninja Warrior. Eliza practising her viola. Just a regular Monday night.

[2018-07-22](/diary/2018/07/22.md)

Jack to NorthShore. Eliza and I teamed up to play "Captain Toad's Treasure Tracker". Then to Van's for lunch; Ba made steak and vegetables. Did some shopping in the afternoon, and made vegetable soup in the Thermomix for dinner. Still early, so Eliza cajoled us into playing Munchkin. She won, of course, but there was no backstabbing (so it was really just a race to the finish). Watched a few episodes of "Handmaid's Tale" with Dzung once the kids were asleep. Again with the lack of HackTile.

[Previous](/diary/page16)Page: 17 of 26[Next](/diary/page18)