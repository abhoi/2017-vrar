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

[gif]
That is clearly a cool concept that was implemented and I have not seen that with any of the other teams (including mine).

## Sound Loop

The second thing I found great was the sound looping. We implemented in our project too, but this team added the ability to pause music instead of just stopping it. My sound loop works on 4 songs and it stops (you can restart), but you cannot pause in mine. The sound controls look pretty decent on the wall to for easy use.

![Spanish Original]({{ site.url }}/assets/spanish_original.JPG)
## Lighting

Thirdly, I like the party mode/disco lighting that was implemented when you hit the button on the wall. They used a custom lighting model instead of the usual point light and what not. That is a really creative use of lighting in a scene. A gif of that:

[gif]
 ## Effective Use of Space

Lastly, the use of the sound room and more to convert into a music room and kitchen was nicely done. The objects there are appropriate. Also, this gives the team an opportunity to fill the scene with more objects.

Final thoughts would be how they also implemented frame rates well. On my laptop, the executable lagged a bit. However, the demonstration on the Vive in the classroom had ample frame-rate and was decent. This was the first project I found particularly good.

![Spanish Original]({{ site.url }}/assets/spanish_original.JPG)
![Spanish Translated]({{ site.url }}/assets/spanish.PNG)

The first image shows the original Spanish text taken from the Camera app. The second image shows the live translation feature Google Translate has. Speaking of accuracy, the algorithm did a fine job in translating the text. However, it was a pretty easy one to do.

## 2. **French to English**

![French Original]({{ site.url }}/assets/french_original.JPG)
![French Translated]({{ site.url }}/assets/french.PNG)

Again, we see a similar situation where a piece of French text needs to be translated. In this case, however, we see the application's lack of accuracy when translating the above text. It does a great job translating the syntactic meaning of the words, but fails to translate its semantic tone.

## 3. **Chinese to English**

![Chinese Original]({{ site.url }}/assets/chinese_original.JPG)
![Chinese Translated]({{ site.url }}/assets/chinese.PNG)

The Chinese text example worked really well considering the amount of text the app had to parse through to translate into English. The accuracy can be considered reasonable for the amount of translation done. One thing to notice in live usage was the frame rate considerably dropped to below 15FPS which is a user experience nightmare.

## Effective Use and Possible Future Use

As of now, Google Translate works reasonably well to translate text from one language to another. We can aim our phone's camera towards a piece of text and have it translated. This also requires an internet connection (but it can be waived by downloading the language pack which is about ~35MB). We can also feed the app an image of text to translate locally. However, this feature is limited to our use of the app within our smartphone. Currently, we do not see the world through our smartphone majority of the time (despite the overgrowing concerns that we definitely are!). Our field of view and vision is dependant on our eyes.

A reasonable assumption for the future can be that we might start wearing "smart glasses" (hint hint [Google Glass](https://www.x.company/glass/)) for the majority of our day. There will be a time when these glasses will be like our smartphone and may overtake our smartphones as the number one electronic device we use. I will refer to any future pair of AR glasses or contact lenses as "The Glass". What happens when "The Glass" dictates its features and usage to us rather than the other way around?

One possible test case could be that this translation feature turns on or off when the application feels is appropriate. In that case, if you are wearing "The Glass", how do you distinguish between real text and overlapped, translated text? How much is the user allowed to control of what is augmented and what is real? These are some ethical/implementation questions we must answer to ensure no malicious activity or "fake" information is conveyed to the user. We can assess the effectiveness of this feature by creating a PRO and CON list.

### PROS

1. **Real time translation** of text without any user interaction or prompts. The user does not have to open any application, input any commands, or press any buttons to have text translate. This also eliminates any delay or lag between the time when the user wants the translation and when the result is presented. Currently, when we translate from the Google Translate app, there is considerable delay between when the text is shown and when it is translated. This lag is amplified when the amount of text to be processed increases

2. **Data collection** for datasets so algorithms can train on them. Many translation algorithms use datasets to train their algorithms that do the actual translation. Google's [Neural Machine Translation System](https://research.google.com/pubs/pub45610.html) uses huge datasets to train the system to increase accuracy of translation. Google uses LSTMs (Long Short-Term Memory) Recurrent Neural Networks in its model. This constant stream of translation would definitely help Google train their model

### CONS

1. **Limited control** for user over content augmentation. The user, supposedly, would not have absolute control over how much of his field of vision would be augmented and how much would be real

2. **Accuracy/Authenticity** of translated/augmented data. Given that recent trends have translations increasing in accuracy, you can never be sure if the translation is 100% accurate. Even some photos I took could not reproduce the original intended meaning of the text with even 90% accuracy. There would be a trust issue between the user and the system

3. **Loss of original data** as the user cannot see what was really there. The user would have to turn off the system or remove "The Glass" itself to actually see what is there in real. That seems counterintuitive at best.

4. **Low performance** assuming today's technology. Finally, the performance would be a great deal of issue. With current tech, Google Translate itself suffers from framerate (< 15FPS) when it encounters more than 5 sentences in a foreign language.

## Final Thoughts

I believe the biggest issue is the amount of control the user should get over how much augmentation takes place when using the device ("The Glass"). Companies might be inclined to limit user control in order to provide a better experience (Apple does this too much), but this would lead to a worse experience for the user in the context of AR and translation.


These are some things to consider about the future of AR and Google translation in specific.
