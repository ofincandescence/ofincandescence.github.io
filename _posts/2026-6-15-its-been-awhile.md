---
layout: post
title: "It's been AWHILE"
permalink: /posts/its-been-awhile
---

# It's been AWHILE

Hi. Apparently we opened our last post sort of like this too, but it's been awhile. Though this time\... a LONG while. So what happened?

Well\... Last time we said we were gonna try some ideas for simpler games that won't take eternity to release. We sort of succeeded at that, because soon after that blog post, we did pick up on a project that we are still working on to this day. Which is exactly why we've been so silent\...

We've been so focused on that project that we haven't really had time to write blog posts. Blog posts take more effort than you think! And this project has always given us something to do, so we, unfortunately, kinda neglected this place\... a lot.

In fact, the only reason why we are writing this now is because we're sick and don't really have the energy to work on the project right now\... Which is unfortunate, but hey, at least we get this blog post.

|

### The Project

Okay, so what about the project itself? Well, issue is it still doesn't really fix the eternity to release problem\...? Well, kinda. It's built around the notion that we can do early release, and update the game over time. So although the project itself may not "fully release" in a very long time, *first* release can actually happen a lot sooner.

The name of the Project is **The Story Machine**, and oh boy, have we done a lot for it. We can't show much here today, mostly because we're sick and partly because we're going through massive codebase changes + basically everything is subject to change at the moment, but overall, it has been our most successful project yet.

To put some things into perspective\... We've been doing a LOT of development in the Godot Engine codebase itself. A fairly major component of The Story Machine is portals, which has been the major driver for most of these changes\...as Godot Engine out of the box really isn't built for portals at all. And even with all our solutions and a substantial amount of stuff added to the engine, things just still weren't working exactly how they should.

|

Which is why, at this point, we are just implementing portal rendering directly into the engine! You may call us crazy, but we do have extensive enough experience in things to pull this off. Even though it requires a LOT of augmentation of the scene rendering pipeline, and even adding new support in the vulkan driver code in Godot <span style="color: grey;">(which was actually the easiest part lol)</span>, we still have most to all of the juicy details of this implementation planned out, down to the details of culling, how renderable objects are individually handled, ect.

See, there are two approaches to this - either render the entire scene again for each portal <span style="color: grey;">(which is what our previous out-of-engine implementation relied on)</span>, or go crazy with stencil testing and do everything in one render of the scene. Initially we were going to go with the former approach again for the in-engine implementation, but the latter just seemed too irresistible. So we're going with that. This would mean, hypothetically, RIDICULOUSLY fast portal rendering, about as fast you can get. So that has us excited. But then we got sick, so\... haha. We are slowly picking up work though.

It may all sound like too much work to handle, but we assure you, we can handle it. We have a fair amount of experience in low-level development like this, particularly in C/C++ which Godot is written in, it's almost like we were built for this. We knew those couple years of writing game engines wouldn't fail us\... Even though we are no longer using a custom engine, we sure have a lot of power over our personal fork of Godot. We feel as if we can do anything. <span style="color: grey;">(Obviously we can't do *everything*, but we have been able to overcome most to all hurdles in our way fairly quickly and overall are very quick to learn the inner workings of Godot Engine.)</span>

|

#### About The Story Machine

Anyway, you might be wondering, what is it about? Well, basically, it's a "walking simulator". Think of something like Yume Nikki, but 3D. It has a Nexus with doors, and you explore several sub-worlds and stuff. However, it's visual style is much further from Yume Nikki, and is a lot closer to Rain World in terms of style. That is mostly because, well, the game has HUGE Rain World inspiration.

Originally, The Story Machine was meant to be in the same universe as HATE IN THE MACHINE (Which A Legend of Shadows is also in), but we decided to separate the two and The Story Machine has its own universe with its own lore.

Overall, we're very happy with where it's going and we aim to do an early release by next year. When next year, we're not sure, but we do want to get it out as soon as we can, even if it'll be in a pre-alpha stage. From there, the game will likely receive regular updates until it fully releases, whenever that'll be.

Part of us is afraid however because, we may not be able to do this alone forever - if the game picks up enough attention, we may have to get additional team members if we want to develop the game at a speed even close enough to satisfy the masses\... We'll see. 

|

Anyway, although we said there's not much we can show in-game at the moment, we do at least have some things we can show right off the bat.

|

<style>
  .centre {
    margin: auto;
    max-width: 512px;
    text-align: center;
  }
</style>

<figure class="centre">
    <img src="/assets/images/the-story-machine/the_story_machine-cover.png" alt="The Story Machine OST Cover">
    <figcaption>The Story Machine OST Album Cover. The way we made this is pretty interesting in itself and may deserve its own blog post at some point.</figcaption>
</figure>

|

<figure class="centre">
    <img src="/assets/images/the-story-machine/logo.png" alt="The Story Machine Logo">
    <figcaption>The current logo of The Story Machine. The text in the logo is actually generated in-game, and if we want to use it in a logo such as this outside the game, we have to export it at runtime. It's pretty funny.</figcaption>
</figure>

|

There will certainly be more to show in the near future. But for now, this is all we can share.

|

### Other Projects?

Bad news, as expected, all other <span style="color: grey;">(creative)</span> projects have been shelved for The Story Machine. I don't think this should be surprising, nor disappointing. It was kind of the whole point of this endeavour, and The Story Machine is definitely by far the most fun thing to work on than everything else so far. We're still considering returning to electrical engineering when we get our disability pension <span style="color: grey;">(they owe us over $8000 worth of back-pay at this point\...)</span>, but all focus will certainly remain on The Story Machine.

There is also our Ardices Glatignyi experiment that we did\... That proved to be successful. A bit too successful? We think that certainly deserves its own blog post, partly because we can't put too much effort into this blog post at the moment, and there's a fair lot to talk about there\...

All we'll say is Thurston, a legend amongst the initial caterpillar generation, did emerge as a moth, mated, and we are currently taking care of his children. In fact, his children are basically as big as he was when we found him last year at this point! Yeah, we were surprised this whole thing worked out so well. We'll at least share a picture of him here before whenever we make that blog post.

|

<figure class="centre">
    <img src="/assets/images/moths/thurston1.webp" alt="Thurston">
	<img src="/assets/images/moths/thurston2.webp" alt="Thurston, Again">
</figure>

|

Sorry about the poor quality. Once again, we may make a proper blog post later. Believe it or not, not much is actually publicly available about this species, including its pupation length\... That information is basically NOWHERE online, so we had to find out ourselves.

Well, after all this time, we can say now that it pupates for roughly 8 months, going into their pupa in late-winter / early-spring and emerging in mid-autumn the following year. This may be the only publicly available resource that mentions the pupation length of this species now, lol. This little blog hidden away in the depths of the internet, containing such obscure knowledge about a moth barely anyone cares about due to its location\...isn't that funny?

We also remember one resource saying there are two generations a year - that's kind of false? The entire lifespan is one year, considering their very lengthy pupation\... We're not sure where that "two generations a year" metric came from. Maybe they mean in a different way than we are imagining.

|

### Other Things

Well anyway, before we go, we want to share a few more things\... specifically music. Not much, but hey, it seems to be tradition at this point, even though this is only the third post <span style="color: grey;">(oops\...)</span>

|

<figure class="centre">
	<audio controls>
		<source src="/assets/audio/Misc/Echoes of Woodpecker, and the Foreboding of the Receiver and City in Secrecy.ogg" type="audio/ogg">
		Your browser does not support the audio element.
	</audio>
	<figcaption >Echoes of Woodpecker, and the Foreboding of the Receiver and City in Secrecy</figcaption>
</figure>

|

<figure class="centre">
	<audio controls>
		<source src="/assets/audio/Misc/Under the Glow of the Storm.ogg" type="audio/ogg">
		Your browser does not support the audio element.
	</audio>
	<figcaption >Under the Glow of the Storm</figcaption>
</figure>

|

Both of these were originally intended as "in-game CDs" for The Story Machine that you could find, but we're not too sure about that idea anymore, or at least if we do have that, they'll be in a different style. Honestly these are both kinda mid, and we aren't happy about the ending of that second one, feels too repetitive\... But it's whatever. We can't be bothered to work on these any further.

|

Welp, that's all for now. Sorry for the lengthy wait between posts\... It was seriously way too long, but we were just too hyper-focused on The Story Machine and still are. So we took this chance to write a blog post when we can. Hopefully it won't be too long before we make another post, because we do feel kinda bad for neglecting this place\...

Anyway, happy, uh, experiencing? May the eternal exhibition forever leave you with interesting qualia.

|

##### - Of Incandescence