[2018-06-30](/diary/2018/06/30.md)

Dzung took the kids to karate, so I spent the morning doing some work. Brunch was Korean BBQ at Van's place, and we overate, so had to move our dinner booking from 6:30pm to 8:00pm. Dropped the kids at Mum and Dad's, then worked on HackTile while Dzung took a nap.

![Sprite Editor](/diary/assets/sprite_editor.png)

Sprite editor taking shape. Created default sprites, and working towards having sprites selectable in the entity viewer. Also need to make entities selectable in the right-hand sidebar, and allow the sprite editor to be shown and hidden through menu items. Also need to support animation and serialization. Then this will be good enough to allow me to move on to the map editor and the rule editor. Exciting times.

Off to Kuzu for dinner, but time to kill before then, so will celebrate with a G&T and some gaming.

[2018-06-29](/diary/2018/06/29.md)

Very busy at work. Beautiful clear day, but so very cold, so didn't go for a bike ride. Fixed the multiple drawing bug from yesterday, and improved the functionality of the sprite editor. The sprite data is now modified too, meaning palette changes work, and it's possible to select the drawing colour. Coming together, but still lots to do. Dinner over at mum and dad's house. All feeling a bit tired, so will call it a night. Might play a game before bed.

[2018-06-28](/diary/2018/06/28.md)

Very busy at work. Eliza off sick. Managed to get some HackTile time; got the sprite editor to a state where I can draw pixels, but there was a funny bug, because I forgot to disable drawing to the world at the same time. I'll need to set an active flag on the cameras too, similar to what I've done with the UI panels. So much more to do.

![Bug](/diary/assets/bug.png)

Meeting with Jack's teacher. We will work hard getting him to improve his concentration and his ability to work unsupervised. Eliza's report came through; she got eight As and has been promoted into the advanced maths track. Good girl!

Made shaking beef for dinner. Will relax before bed with The West Wing, wine and cheese. Oh, and I ordered the new TV. Should be delivered soon.

[2018-06-27](/diary/2018/06/27.md)

Well, not in a rut after all. Early morning meeting at work, then needed to work on getting the builds of all apps in order. While waiting for the builds to finish, I read my new C book and finished the refactoring work, and then mocked out the layout for the entity viewer and sprite editor.

![Mock UI](/diary/assets/mock_ui.png)

The idea is that the red bar on the right will contain controls for selecting one of 32 entities, and for showing dialog boxes for editing various aspects of the simulation. The blue dialog on the left will show up to eight animations for the currently selected entity; idle, four directional animations, spawn and unspawn, and a special emote animation. The green dialog on the right will allow the currently selected animation to be edited. Each animation has up to three frames, each consisting of a 16x16 bitmap.

That's the idea, anyway. We'll see how it pans out.

This morning Dzung and I went to the school, in the drizzling rain, to watch Jack run cross-country. About half the boys try their hardest. Jack gets distracted, and decides to walk and muck around with his friends. Frustrating!

Tonight Eliza and I made lamb, pea and mint pasta. It was nice and filling, and tasty too, but not as good as the other dishes we've made. Watched some MasterChef after dinner, then read "Magician's Gambit" to Eliza. She had a bit of a tummy upset. Then a bit more work before cleaning up while listening to The West Wing Weekly before heading to bed.

[2018-06-26](/diary/2018/06/26.md)

Up early. Did some work. Made breakfast and lunch. Took kids to school. Back home to bacon and eggs and some reading before working some more and going for a mid-morning ride around the river. Afternoon business call, then picked up the kids and off to swimming lessons. Then into the city for a pubby dinner at Butcher's Arms and a look at the light installation in the city.

"C in a Nutshell" arrived today, and I did some refactoring of code based on the C11 standard as a result. Expect to refactor some more tomorrow, and continue on the editing UI. Feel like I'm entering another rut. Sigh.

[2018-06-25](/diary/2018/06/25.md)

Up early. Made breakfast and lunch for the kids. Beautiful morning, so walked Jack in once Dzung was back from dropping off Eliza. Regular day at work. Took a break mid-morning to ride two laps around the river and soak in the nice weather. Reheated some soup for lunch, Dzung and I read our books outside in the sunshine. Then walked in to school to get Jack, picking up a few groceries on the way home. He got his report today; Bs in Maths and Japanese, but Cs for everything else. We'll need to work on improving those grades!

Picked up Eliza after quiz club. She complained of a headache. Kids good, Jack did some homework and some reading. He tries hard. Eliza did hers. I managed to squeeze in some HackTile work; got a PanelManager implemented, with a few placeholder panels rendering where the editor UI will be. Should be able to flesh them out over the next few days.

Made grilled pork steaks with roasted sweet potatoes in a lemon butter sauce, garnished with parsely and red onion for dinner. Eliza helped. Delicious! Put both kids to bed, reading to them both (I downloaded an illegal PDF of Magician's Gambit, since they pulled it from the Kindle store). Dzung cleaned up, so with nothing left to do I'm having an early night reading in bed. I'm enjoying this cruisy approach to hobby projects, chipping a little off each day rather than burning the candle at both ends.

[2018-06-24](/diary/2018/06/24.md)

Busy day. Finished making the lamb and barley soup that I started last night, and went to the shops to grab salad, cheese and frozen chips. Then prepared soup, hamburgers, chips and salad for Dzung's side of the family. Beautiful sunny day, so we sat outside to eat. Ma had two lamb sliders, and Ba ate several bowls of soup, and asked for some more to take home for dinner. Success!

Lilian, Lachlan and Joshua played their violins for us afterwards. Then packed up and went to pick up Mum and Dad to take them to the Civic Centre in Cottesloe where we watched Eliza and Jack's piano concert. They played with confidence. Very proud of our kids. Finished the day at Barchetta, watching the sun set over the ocean. Ordered pizza and a share plate, and wine and beer.

Did a little bit of work on HackTile but nothing much. Need to find time during the week, as I'm pretty tired now and will make it an early one.

[Previous](/diary/page20) Page: 21 of 26 [Next](/diary/page22)