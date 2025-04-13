[2018-07-07](/diary/2018/07/07.md)

Strong coffee and crumpet breakfast once the washing was on, happily flicking through new issues of The Guardian and New Scientist. Then off to karate with the kids, picking up seafood chowder and crusty baguette for lunch on the way home. Lazy afternoon, then dropped the kids to mum and dads. Picked up Annie for dinner at Tiny's. We ordered far too much. Then to the jazz festival to see the Perth Jazz Collective at His Majesty's. Back home to watch Endeavour with a cuppa.

[2018-07-06](/diary/2018/07/06.md)

Kids slept in until eight thirty. Breakfasted, then packed up and cleaned up, and visited our friends to say goodbye. Kids wrote in the guestbook, after discovering their guestbook entry from 2016 the other day. Left a bit later than planned, and I was a bit stressed out, as I'd arranged to have the TV delivered at one o'clock and I was clearly not going to make it. Needn't have worried though, after arriving home and putting everything away the delivery driver called to say he was coming around. Perfect timing, really. Spent the afternoon catching up on work and setting up the TV. Dzung took the kids shopping and to the library, so Jack could get some more books for his reading challenge. Will have can chua for dinner, and will then most likely watch a movie on our new sixty-five inch idiot box.

[2018-07-05](/diary/2018/07/05.md)

Last full day. Kids were freezing cold overnight. Made bacon burgers for breakfast and had an easy morning. Dzung walked the dog with the kids and went to say hello to the alpacas while I chopped wood. Drove into Nannup to get pies and pasties for lunch, then went for a walk along the Blackwood River. Back home to light the fire and hop into the spa. Roasted some vegetables for dinner and cooked the lasagna. Played a few rounds of Resistance then had an early night with electric blankets on for everybody. Almost finished reading "The Seven Deaths of Evelyn Hardcastle".

[2018-07-04](/diary/2018/07/04.md)

Slept great. Strong coffee and raisin toast for breakfast. Headed into Bridgetown for lunch. Whole place has been decorated with ornaments woven from white wool to make it look like a winter wonderland for Christmas in July. And amazed to find the puzzletown exhibition, featuring countless jigsaw puzzles, including the smallest and largest in the world. Fantastic lunch at the Barking Cow cafe. Had planned to go bushwalking but the weather set in so we grabbed groceries and filled up with petrol before driving back to the chalet to light the fire. Dzung and the kids made a start on the jigsaw puzzle they bought while I read, then over to Nagis and Ali's for a dinner of fish, wild rice, veges and salad. Kids did a hilarious magic show performance. Walked home in the cold dark night to a guttering fire that I resurrected before ending the evening in the hot tub. Electric blankets set to max. Love relaxing and spending time away from screens, would love to live like this and work on HackTile when inclined, with lots of bushwalking to think.

[2018-07-03](/diary/2018/07/03.md)

Worked in the morning but no time for HackTile. Dzung had to go in to the office to demo her project, so I organised the kids and got things packed up. Nice drive down to Nannup. No rain to speak of; we were lucky to miss the stormy weather. Great to be back amongst the big trees. Arrived and settled in, then over to visit Nagis, Ali and Nora (and Hora the dog, of course). Then back to our chalet to cook lamb cutlets and pasta for dinner. I'm doing dry July so missed the red wine. Played a bit of Resistance after eating, then ended the night in the hot tub. Glad to have a roaring log fire to keep us warm after getting out of the water!

[2018-07-02](/diary/2018/07/02.md)

First day of the school holidays. Cold and rainy. Did some activities with the kids; filmed Eliza doing her piano levels and helped Jack with his reading, but overall a busy day at work fixing the Android builds. Break at lunch to go shopping for holiday supplies, and to grab pies for lunch. Did some reading of the "Bullshit Jobs" book, which I agree with wholeheartedly. Dzung home to make soup and grilled pork with rice for dinner. Watched an episode of "Back in time for Dinner" with the kids while eating apricot yoghurt for dessert. It was the 1970s episode, and brought back a lot of childhood memories.

Kids to bed and then some HackTile work. Refactored the camera system to make zooming a lot more sane. Works well, although there is a limit to how far you can zoom out (to do with overflowing integers). Added keyboard controls to zoom in and out. Will need to refine this after returning from Nannup so I can move on to finishing the map editor. Will have lots to think about while bushwalking.

[2018-07-01](/diary/2018/07/01.md)

Finlay's seventh birthday. Kids at mum and dad's, so Dzung and I were mooching around in our PJs when Eliza's English teacher arrived to deliver the book she needs to read for the holidays. Embarrassed! Off to Imperial Court for Dim Sum. They had a large function there, but we were lucky to get a table for thirteen in the back room without waiting too long. Lazy afternoon at home, ended up playing Zelda:BotW with Jack for an hour or so after a simple Sunday dinner of leftover soup and toasted cheesey bread.

Lots of work on HackTile. Entity editor layout updated, and sprite selection working properly to allow editing of any sprite, with a keyboard command to show and hide the editor, and the ability to select any entity for editing and for drawing into the map. Need to sort out camera controls next, so I can pimp out the map editor a bit more, and will also need to address animations.

Unfortunately I've had a re-think about how to assign sprites to entities, so I'll need to re-do my default sprites and a bunch of code. This happened because I think movement animations will need to be three frames. So it'll be:

- 8 entities with 16 sprites (12 for movement, 2 for spawn, 2 for unspawn)
- 8 entitries with 8 sprites (4 for movement, 2 each for spawn and unspawn)
- 8 entities with 5 sprites (1 default sprite and the spawn/unspawn ones)
- 8 entities with just 1 sprite

This still leaves me with the 16 reserved sprites I need for UI things.

[Previous](/diary/page19) Page: 20 of 26 [Next](/diary/page21)