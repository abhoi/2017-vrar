---
layout: post
title: Microsoft Holoportation Critical Analysis
published: true
---

## What is Microsoft Holoportation?

Microsoft’s [Holoportation](https://www.microsoft.com/en-us/research/project/holoportation-3/) project works on the principle of capturing 3D models of real life objects (especially humans!) and reconstructing them in a space visualized by another Microsoft Hololens. Microsoft categorizes their Hololens as **mixed reality** instead of augmented reality now. With this amazing implementation, it is hard to argue against it. A working demonstration of the application can be viewed here:

[![Holoportation](http://img.youtube.com/vi/7d59O6cfaM0/0.jpg)](https://www.youtube.com/watch?v=7d59O6cfaM0)

Even though this is impressive, what they accomplished next is even cooler. They created a system to achieve the same functionality in a mobile setting! That just means they got Holoportation working from a car. A working demonstration of that can be found at:

[![Holoportation2](http://img.youtube.com/vi/nTkFO2xNkIk/0.jpg)](https://www.youtube.com/watch?v=nTkFO2xNkIk&feature=youtu.be)

I believe the most impressive feat is that they accomplished the mobile version of Holoportation with just two cameras. The cameras capture depth information for 3D model generation. Although, I believe more cameras would provide them with more information resulting in a 3D model that is more realistic. Another challenge they faced was the bandwidth issues. The Microsoft team behind this says they solved the challenge by reducing bandwidth requirements by **97% to 30-50MBps**.

## Critical Analysis

Let us go into more detail about what is great about this project and what can be improved with more research. Before we do, I strongly suggest you read  the [paper](http://www.cs.toronto.edu/~slwang/holoportation.pdf) by **Escolano et al.** behind the project. First, we’ll explore the positives.

1. The application works exceptionally well with **still**, 3D objects such as chairs or desks. Even small objects like toys and laptops get reconstructed really well. When it comes to humans, the application does a good job. There may be some inaccuracies, but the way the application tracks is impressive.

2. The tracking system works on the basis of **fusing** different camera viewpoints into **meshes** to be reconstructed temporally. 

3. The team also succeeded in pushing through huge amounts of data (different camera feeds will increase the amount of data to be processed and transmitted dramatically) with **limited** bandwidth.

4. **Audio source and volume** is relative to the user’s position and orientation instead of being completely stereo or mono. That means, wherever the 3D model is constructed, the audio emits from that location instead of some random location or all over the place.

5. The **depth estimation and segmentation** based on masking and color RGB extraction provides an accurate representation of the object from each camera view.

One thing to notice is that this is neither completely augmented reality nor completely virtual reality. This is a mix of those two combined into “mixed reality”. This is because you view the object that is constructed using principles of VR but viewed in an AR scene.

### What can be improved or has potential to grow?

1. The 3D model construction, especially for humans, is **not** perfect and often approximates data in order to construct the model. It can be made better using better segmentation techniques. However, this would require more bandwidth.

2. There is **notable latency** with respect to what the user did at one place and what another use sees at another. This can be improved using a better GPU pipeline to push data through and process it faster. Better network pipelines can also help with lowering the latency.

3. Models are **not interactable**. This is a tough one as it is very difficult to approximate weights and bodies to 3D models and make them interactable to a user.

With the technology being just over one year old, I believe there is much more space for the technology to grow before it becomes mainstream and be consumer usable. People adopt technology that is easy to use and “cool” to use. I think the application has many hurdles to overcome before they achieve that goal. The whole pipeline of this Holoportation technology can be visualized as:

[image]({{ site.url }}/assets/holoportation.PNG)

## Collaboration

Two possible uses for this kind of technology with respect to collaboration can be categorized into **one-to-one** (doctor-patient visits, educational instruction, personal meetings) and **one-to-many** (sporting events, business meetings, collaborative events).

Imagine a scenario with a remote village that requires medical assistance but is blocked off due to some natural calamity (perhaps a storm). In that case, it is terribly difficult for a doctor to come to the village to diagnose the patient and even more difficult for any village member to travel to the doctor. In cases where physical presence is required and the medium is not present, Holoportation can provide a way for the doctor to diagnose or even checkup on the patient remotely.

Another scenario can be something that would save companies millions of dollars. Consulting firms usually spend millions every year flying out their directions and technical leads to client sites, office locations, or even storage warehouse facilities. Most of the times, it is for the employee to interact with someone physically in order to either provide importance, make sure face-to-face, or just involve the members more. However, instead of wasting so much money on air tickets, hotels, and transportation charges, companies can instead utilize Holoportation to virtually construct a meeting space for employees and clients so that they can interact on a more personal level (not skype nor phone calls) and still stay local.

Holoportation mobile extends this idea of collaboration **on the go**. This can work, however, more limitations such as bandwidth and processing power need to be overcome for this to be appropriately usable.

## Tracking and Cameras

Speaking of tracking, Microsoft did something that people are working (including my team!) on since last year. The concept of constructing or generating 3D models (or tracking objects) temporally without losing data in between or without **“temporal flickering”**. Instead of just visualizing data points in point clouds from multiple cameras, the team fused the data to generate one mesh per frame to reduce noise level. This might still suffer from flickering effects, so, they created a novel method to track meshes and **fuse data across cameras and frames**. The paper linked above dives into more detail about this.

## Interaction

With everything going on in this project, interaction, unfortunately, is **not** supported as of yet. For example, you can record the mixed reality sessions you had with another user and view them later whenever you feel like. However, there currently is no way to interact with the 3D constructed models. This one challenge would solve many user interface problems, however, the challenge is a tough one. This would require generating even a more detailed 3D model instead of simple meshes. Then you would need to assign some rigid bodies and colliders to the model to make them interactable.

One can imagine the possible interactions though. You could shake hands with the other person, throw around objects in the mixed reality world, or even save some objects for later use. Microsoft’s other [projects](https://www.microsoft.com/en-us/hololens) have worked on augmented reality where  users can pin objects. Perhaps, they can port that technology to this one.

Overall, Holoportation is a great piece of invention and has lots of things to check off before it can truly become revolutionary. Still, it is one of the biggest steps forward in the field of mixed reality, augmented reality, and virtual reality.
