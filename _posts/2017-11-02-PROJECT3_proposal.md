---
layout: post
title: Project 3 Proposal - ARYouThereYet
published: true
---
## ARYouThereYet

The application we are developing is an Augmented Reality application usable primarily for walking navigation. 

### General Description

The primary features we aim to implement in the application are:

1. Insert a HUD popup of basic information about places in current camera view with following information:
	- Place Type Icon
    - Place Name
    - Distance from current location in miles
2. Click on desirable popup to view more information about the place including:
	- A descriptive picture of the place
    - Description box with quick description of the place
    - Picture collage to view more pictures
    - Navigation button to enable navigation view
    - Share button to open Apple sharesheet (can share location)
    - Reviews of the place (out of 5 stars)
    - Context aware box that changes content based on type of place (events, shows, movies, etc)
3. A navigation view when clicked on desired location that has 3D arrows leading to the destination.
4. Dynamically filter places you want to see in the ARScene view.

### Hardware Platform

Our application will be developed primarily for the Apple iPhone. Specifically, ARKit supports any iPhone with an A9 processor and above. That translates to iPhone 6s and any iPhone released after that.

### Software

The application is going to be built using [Apple’s Xcode IDE](https://developer.apple.com/xcode/), [ARKit framework](https://developer.apple.com/documentation/arkit), and [Google Maps API](https://developers.google.com/maps/) and [Google Places API](https://developers.google.com/places/).

### Team Member and Responsibilities

1. **Amlaan Bhoi** will be responsible for data management including structuring API calls, parsing relevant JSON data, creating data modals, and instantiate relevant data objects. He will also work on ARKit and Vision framework.

2. **Sandeep Joshi** will primarily be responsible for ARKit development with respect to 3D model generation, HUD development, tracking objects based on location data, and more.

3. **Debojit Kaushik** will be responsible for UI element design, scaling/sizing of elements based on constraints, development on ARKit, and implementing extra features.

### Datasets/Libraries

Our data will primarily be sourced from:

1. **Google Maps API:** [https://developers.google.com/maps/](https://developers.google.com/maps/)
2. **Google Places API:** [https://developers.google.com/places/](https://developers.google.com/places/)

![Demonstration]({{ site.url }}/assets/ar2.gif)
