---
layout: post
title: Thoughts on Google Translate and AR Issues
published: true
---

# **Google Translate**

Google Translate ([translate.google.com](http://translate.google.com)) is considered the gold standard for translation between various languages. It is not surprising to see the addition of "live translation" aka "image translation". This feature succeeds in segmenting an image or live camera feed and recognizing foreign characters. Not only that, it also succesfully supersedes the original text with an English translation (assuming foreign language to english translation is required)!

Let us first see three examples of such translation that I took in various locations on West Taylor Street here in Chicago.

## 1. **Spanish to English**

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

The Chinese text example worked really well considering the amount of text the app had to parse through to translate into English. The accuracy can be considered reasonable for the amount of translation done. One thing to notice in live usage was the frame rate considerably dropped to below 15 fps which is a user experience nightmare.

## Effective Use and Possible Future Use

As of now, Google Translate works reasonably well to translate text from one language to another. We can aim our phone's camera towards a piece of text and have it translated. This also requires an internet connection (but it can be waived by downloading the language pack which is about ~35MB). We can also feed the app an image of text to translate locally. However, this feature is limited to our use of the app within our smartphone. Currently, we do not see the world through our smartphone majority of the time (despite the overgrowing concerns that we definitely are!). Our field of view and vision is dependant on our eyes.

A reasonable assumption for the future can be that we might start wearing "smart glasses" (hint hint [Google Glass](https://www.x.company/glass/)) for the majority of our day. There will be a time when these glasses will be like our smartphone and may overtake our smartphones as the number one electronic device we use. I will refer to any future pair of AR glasses or contact lenses as "The Glass". What happens when "The Glass" dictates its features and usage to us rather than the other way around?

One possible test case could be that this translation feature turns on or off when the application feels is appropriate. In that case, if you are wearing "The Glass", how do you distinguish between real text and overlapped, translated text? How much is the user allowed to control of what is augmented and what is real? These are some ethical/implementation questions we must answer to ensure no malicious activity or "fake" information is conveyed to the user. We can assess the effectiveness of this feature by creating a PRO and CON list.



The plethora of augmented reality (AR) applications found on most smartphones/tablets today includes apps such as Quiver ([quivervision.com](http://www.quivervision.com)), Pokémon Go ([pokemongo.com](http://www.pokemongo.com)), and even Google Translate ([translate.google.com](http://translate.google.com)).
## Advantages

   (a) **Portability**: Phones and tablets are ultra-portable and allow users to move about, wander, and explore large areas without any major restrictions (battery life is an exception). AR apps running on these devices makes these apps portable as well.

So these are the various AR/VR platforms and their respective advantages and disadvantages. A doc version of this post can be found at [WEEK1_ARVR_comparison](https://www.dropbox.com/s/1sing3rtt7rn99q/WEEK1_ARVR_comparison.docx?dl=0).
