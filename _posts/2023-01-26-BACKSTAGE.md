---
title: A Quick Tour of the Machine Room
date: 2019-08-08 14:10:00 +0800
categories: [Conceptual]
tags: [IDE, GitHub, Frontend]
render_with_liquid: false
pin: true
---

Upon visiting my website, I hope you were delighted by its design, simplicity, and delivery of content. This post is for you if you would like to get a glimpse of the technical concepts I use to develop and maintain this website.

## Requirements

Before starting off the implementation of the website, I had clear non-functional requirements in mind which this project must meet:

* Since 'the prevention of re-inventing the wheel' is a key challenge every developer ought to tackle in his daily life, the website must be based on a reusable, open, and well-maintained framework.
* The website should be developed and maintained using some sort of `Git` flow, where the `dev` environment closely follows the `prod` environment. Moreover, the `dev` environment provides comprehensive testing capabilities.
* The website should allow for creating visualisations programmatically; that is to say visualisations should, whenever possible, be based on code instead of powerpoint screenshots.
* Web hosting should be easy-to-use and inexpensive.
* Since I am travelling and I don't have my laptop with me, all of the above can be done from an iPad (yikes).

Needless to say, doing codework from an iPad is pretty uncommon... unheard of in my case: I have never met anyone before who has used an iPad to do proper development on an iPad. However, this challenge made me go out of my >5 years MacBook-based developer comfort zone, and I am really happy with the new tools and technologies I have learned thanks to my current situation.

## The Machine Room

* All codework is done from `GitHub`'s built-in `Codespaces` service, representing a remote version of `Microsoft`'s `Visual Studio Code`. This way, all technical work is seamlessly integrated in the `Git` flow I have defined for this project. Moreover, just like `Visual Studio Code`, `Codespaces` comes with a `Terminal` which allows for building and testing the website in its `dev` stage.
* 