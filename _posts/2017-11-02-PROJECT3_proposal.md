---
layout: post
title: Project 3 Proposal - ARYouThereYet
published: true
---

The application we are developing is an Augmented Reality application usable primarily for walking navigation. In today's world, when we travel to unknown places or are just looking for something fun while exploring the city, we often get lost and are unable to locate where we are. Maps such as Google Maps or Apple Maps do a good job coordinating us towards a destination, but they are not intuitive at all and often confuse us even more. The primary motivation for us to develop this application is to bridge this gap by creating an intuitive and immersive experience for the user by using the power of Augmented Reality and overlaying virtual objects onto the real world in order to make more sense of what is around us.

### Storyboard/UI Concept

Following are some hand designed views we believe are appropriate for the application. These include UI design as well as the different views that will be created for the application specific to what is being done by the user:

![p3_1]({{ site.url }}/assets/p3_1.jpg)

The second one goes into more details of the **"Detailed view"** and **"Filter view"**. Note, none of this is final and more things will be added/removed based on feasibility, appropriateness, and functionality wise:

![p3_2]({{ site.url }}/assets/p3_2.jpg)

A minimal inspiration for the navigation view is inspired by Andrew Hart's [project](https://github.com/ProjectDent):

![Demonstration]({{ site.url }}/assets/ar2.gif)

Lots more detail and better looking 3D models will be used instead of the stock shapes.

### General Description

The primary features we aim to implement in the application are:

1. Insert a **HUD popup** of basic information about places in current camera view with following information:
	- Place Type Icon
    - Place Name
    - Distance from current location in miles
2. Click on desirable popup to view **more information** about the place including:
	- A descriptive picture of the place
    - Description box with quick description of the place
    - Picture collage to view more pictures
    - Navigation button to enable navigation view
    - Share button to open Apple sharesheet (can share location)
    - Reviews of the place (out of 5 stars)
    - Context aware box that changes content based on type of place (events, shows, movies, etc)
3. A **navigation view** when clicked on desired location that has 3D arrows leading to the destination.
4. **Dynamically filter places** you want to see in the ARScene view.

### Hardware Platform

Our application will be developed primarily for the **Apple iPhone**. Specifically, ARKit supports any iPhone with an A9 processor and above. That translates to **iPhone 6s** and any iPhone released after that.

### Software

The application is going to be built using **[Apple’s Xcode IDE](https://developer.apple.com/xcode/)**, [ARKit framework](https://developer.apple.com/documentation/arkit), and **[Google Maps API](https://developers.google.com/maps/)** and **[Google Places API](https://developers.google.com/places/)**.

### Team Member and Responsibilities

1. **Amlaan Bhoi** will be responsible for data management including structuring API calls, parsing relevant JSON data, creating data modals, and instantiate relevant data objects. He will also work on ARKit and Vision framework.

2. **Sandeep Joshi** will primarily be responsible for ARKit development with respect to 3D model generation, HUD development, tracking objects based on location data, and more.

3. **Debojit Kaushik** will be responsible for UI element design, scaling/sizing of elements based on constraints, development on ARKit, and implementing extra features.

### Datasets/Libraries

Our data will primarily be sourced from:

1. **Google Maps API:** [https://developers.google.com/maps/](https://developers.google.com/maps/)
2. **Google Places API:** [https://developers.google.com/places/](https://developers.google.com/places/)

More information sources may be added as needed and everything is purely dynamic with nothing being hard-coded.

This is the proposal for Project 3 which we believe is applicable, useful, and a great addition to the AR community!


