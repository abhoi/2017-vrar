---
layout: post
title: Comment on Project 1 (Other Teams)
published: true
---
In this post, I will download, run, examine, and comment on other projects submitted for PROJECT 1 in the CS 491 - Virtual and Augmented Reality class. The two projects I have selected are ones I found well implemented and carefully thought out. This review is more of a personal comment than a formal review.

Let us explore start with the first project I found awesome!

# 1. TEAM 1 (Amico, Simone | Foglio, Matteo | Milanta, Andrea)

At first glance, the scene of their project looks simple and similar to every other project in the class. However, at closer inspection and probing, the project seems to deliver new concepts not mentioned in the project requirements. Before going into too much detail, the team implemented some really cool concepts such as music looping through wand interactions, GameObject creation through colliders, custom lighting, and extension of two rooms in a singular classroom. Let us go into details as to how.

## Interactions

Firstly, I love how they managed to implement GameObject creation with the Coke vending machine. Whenever you tap on the Coke vending machine button, a coke bottle drops from the machine. That would be creation of a GameObject when some interaction is done. Why don’t we see that through a gif interaction instead of an image:

![Vending Machine]({{ site.url }}/assets/project1_review/coke.gif)

That is clearly a cool concept that was implemented and I have not seen that with any of the other teams (including mine).

## Sound Loop

The second thing I found great was the sound looping. We implemented in our project too, but this team added the ability to pause music instead of just stopping it. My sound loop works on 4 songs and it stops (you can restart), but you cannot pause in mine. The sound controls look pretty decent on the wall to for easy use.

![Song Control]({{ site.url }}/assets/project1_review/sounds.png)

## Lighting

Thirdly, I like the party mode/disco lighting that was implemented when you hit the button on the wall. They used a custom lighting model instead of the usual point light and what not. That is a really creative use of lighting in a scene. A gif of that:

![Lights]({{ site.url }}/assets/project1_review/lights.gif)

 ## Effective Use of Space

Lastly, the use of the sound room and more to convert into a music room and kitchen was nicely done. The objects there are appropriate. Also, this gives the team an opportunity to fill the scene with more objects.

![Whole Room]({{ site.url }}/assets/project1_review/whole_room.png)

Final thoughts would be how they also implemented frame rates well. On my laptop, the executable lagged a bit. However, the demonstration on the Vive in the classroom had ample frame-rate and was decent. This was the first project I found particularly good.

# 2. TEAM 2 (Jyothula, Sai Priya | Sakhnini, Nina)

The second team project I found innovative and well implemented is the project by Sai Priya and Nina. This project is simple and well made. There are many interactions to play around with and all of them have a functional use rather than just an aesthetic appeal. Some of the things I loved was that you can remove the roof (which I will get to), you can pickup individual chess pieces (our project just picks up the entire chess board), and the effective use of space with respect to work cubicles in the middle of the room.

## Interactions

The first interaction that I love is the way the roof opens up when you trigger into the switch in the left side of the room. The switch is located besides another switch which turns on/off the main light source in the room. The roof opening/closing is also accompanied by a sound trigger. The only thing I did not like about this implementation though is the fact that the roof disappears immediately. The sound trigger suggests the roof is sliding in or out of the ceiling. However, the roof simply disappears in this implementation. That is okay and can be built upon. A gif with these interactions:

[gif]

The second interaction I liked was you can pick up individual chess pieces. The implementation requires a box collider on each of the chess pieces. I believe box colliders do not use that much processing and thus the frame rate was saved. Had they used mesh colliders, the application would have been painfully slow or would have crashed. An image of the colliders and a gif is below:

[chess]

[gif]

## Sound Triggers

Almost every actionable item in the scene has a sound trigger attached to it which is pretty cool. The speakers have bongo music playing, going near the cat makes a meow sound, and the aquarium has a bubble noise when you go close to it. One thing I believe that could be improved is the effective range of these items. For the speakers to work, I have to literally go through the speakers (this is specific to when testing the application on a laptop because you could just touch the speaker using the wand on a HTC Vive).

## Effective Use of Space

The last thing I liked about this project is the effective usage of space. Every part of the room has a dedicated space with a meaning. The front of the room is the meeting area (with the roof placed strategically over it), the middle is the working area with cubicles or polygons, and the rear of the room is the enjoyment area with speakers, water fountain, and chess board.

[image]

All in all, the project is really well made with simple concepts and well executed implementations.

These are the two projects I found well made and worth a good grade!