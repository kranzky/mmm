[2018-06-23](/diary/2018/06/23.md)

Up early to buy brioche burger buns from Garden City before they sell out. Then back to get the kids breakfast and take them to karate. Dzung took Eliza to buy a viola while Jack had his lesson. Home via garbo again, this time to pick up lunch for the kids and to get premium hamburger meat. Kids got dressed and we went in to Supanova. Finlay had the time of his life!

![Supanove](/diary/assets/supanova.jpg)

Dropped Fin at mum and dad's in the late afternoon. Stayed for a cuppa and a some rocky road. Then in to Hayashi for a wonderful dinner (superior beef, vegetable tempura, sous vide salmon, clam miso soup, rice, beer, lotus chips). Back home to make lamb and barley soup for tomorrow, using leftovers from last week's roast. Finished reading Queen of Sorcery to Eliza, and miffed to find that the series has been pulled from the Kindle Store. Wrote an email to PRH UK to ask for an explanation.

Did a little bit of HackTile work; added an overlay renderer and used it to add a transparent background to debug displays. Need to soldier on and get this UI built out over the next week!

[2018-06-22](/diary/2018/06/22.md)

Morning meeting. Light day at work. Went shopping at lunch time to pick up groceries and beer, and to get the new Mario tennis game. A bit of HackTile in the afternoon; refactoring to add two game modes that can be toggled between, and starting to build out controls for the UI. This work will take a while.

Finlay over for a sleepover. I made tortillas. Everyone watching Hotel Transylvania 2 while I read End of Watch. Will have an early night.

[2018-06-21](/diary/2018/06/21.md)

Another busy day at work. Lots of HackTile design, but no programming. Plan to introduce two states; a game state and an editor state, and toggle quickly between them. The editor will have a fixed layout, with the entity and rules editors implemented as pop-up dialogues. That gives me something to start with; refactoring to support multiple states will take a bit of work, and the editor layout can then be implemented with placeholder content, and I can then start fleshing out just the entity editor. Should work fine. Still need to stew on it for another day or two before I roll up my sleeves and start implementation.

Dzung made leftover curry for dinner, I cooked some lamb cutlets to pad it out. She's feeling sick, and there's still a bit of meh-ness around. Forgot to put the bins out last night; another symptom of our general malaise at the moment. I'm going to watch an episode of The West Wing and call it a night.

[2018-06-20](/diary/2018/06/20.md)

Bit of a meh kind of day. Eli came over early, as his mum and dad both needed to be in the office early. He and Jack are obsessed with minerals. They examined Jack's rock collection enthusiastically, and were fascinated when I set up the digital microscope for them to use. After school, Jack made "Brentwood Geologist" membership cards for himself, Eli and Josh, which I helped him print and laminate. Great to see them obsessing over something!

Watched the lap-a-thon in the afternoon, which Dzung volunteered at. Made bolognaise for dinner. Sat on the sofa and watched three episodes of Seinfeld after dinner. Don't know why, it was just part of the overall meh-ness of the day. I think it started when I woke up bright and early for this morning's team meeting and nobody showed up. Also the comedown after the intense work setting up new customers.

Did some HackTile work; got alpha blending working for sprites. Really has a big performance hit; barely hitting 100fps when maxing things out now. But it's necessary, as I want to have multiple layers. Spent some time thinking about the sprite editor, sketching out some UI designs based on SEUCK. I think I need to stew on this for a few days before coding anything up. I want to keep the editor simple, so making it opinionated is key. One way of doing this is to impose tight constraints on flexibility; limiting the exact number of entities and how they can be used, for example.

[2018-06-19](/diary/2018/06/19.md)

Very busy day at work struggling with builds. Not fun. Day was grey and miserable. Jack's lap-a-thon cancelled due to weather. Dzung made sweet and sour fish for dinner, to use up leftover coriander and spring onion. Delicious.

Switched to a new font for debugging, and made sure the font colour changes with the palette. And got sprites rendering from the hard-wired pixels into a texture buffer to update with the palette too. Need to get alpha working next, then on to a basic sprite editor so I don't need to design these in hex digits.

![Sprites](/diary/assets/sprites.png)

Will end the night with a bit of Zelda, cheese and brandy. Time to celebrate.

[2018-06-18](/diary/2018/06/18.md)

Grey Monday morning. Jack complaining of a sore tummy. Slow day at work struggling with Android builds and getting new apps set up on TestFlight. Picked up the kids and Jack made MaPu ToFu for dinner. Eliza got hit in the head with a basketball at school but took it stoicly. Later she cried when I read her the final chapters of The Queen of Sorcery.

Reimplemented the debug font for HackTile, using a caching library. Debug rendering now incredibly quick, exceeding 300fps when vsync is disabled, event when maxing out the engine. And implemented the beginnings of the sprite manager, to the point where drawing squares of flat colour has been replaced with blitting images from a sprite sheet. Still lots of more work to do there, and I feel that the next step will be implementing a basic sprite editor.

Watched an episode of The West Wing at lunch. Plan to watch another before bed, as Dzung is working and I'm not ready to hit the hay.

[2018-06-17](/diary/2018/06/17.md)

We all had a bit of a sleep in. Late breakfast with the kids, then busy preparing roast lamb, potatoes, carrots, beans, brussel sprouts, salad, gravy and so on. Meat was a bit overcooked but delicious all the same. Ba raided our kafir lime tree for the restaurant as usual. Quickly packed up then over to Elaine's for Mahjong with Josh, Annie and Mitzi. I worked on HackTile while Jack played Zelda and Dzung and Eliza played Mayjong with the others. Got mouse drawing working, and Eliza had a ball trying it out!

![Funny Face](/diary/assets/funny_face.jpg)

Amazing how much fun things are when you can interact. Had dinner at a nearby Thai place, before taking the kids home, leaving Dzung to play with the others. Jack and Eliza mucked around with HackTile a bit once we were home, then it was off to bed. And I'm exhausted, so an early night with "End of Watch" for me.

[Previous](/diary/page21) Page: 22 of 26 [Next](/diary/page23)