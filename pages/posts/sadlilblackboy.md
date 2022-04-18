---
title: Sadlilblackboy Website
date: 2022/4/14
description: Detailed description of the development of the Sadlilblackboy artist site created in Typescript with Gatsby.
tag: web development
author: Quentin Jones
---
# Sadlilblackboy Artist Website

## Introduction
As a musician in the digital age, a landing page is critical for converting listeners and followers to customers generating revenue through digital sales. Throughout an entire muscians career, social media, streaming platforms, and distribution styles will always change; this makes it critical to have a consistent landing page for your audience to be able to find your content.

## Under The Hood

- Gatsby.js
- Typescript
- Netlify for hosting

talk about gatsby image optimization or something. Bring up challenges with netlify and typescript so it seems like I worked really hard idk

## Design Decisions
For any creative platform, the design can be equally important as the content. So, when creating this site, the two key concepts were to make the site both **grappling** but still keep the content **accessible.** These focuses kept me from over-designing and scaring off users who were unable to find the content and products they were looking for.

### Version One (starting out)
Initially, I found it most useful and efficient to have one long scroll of content. 90% of users were visiting on mobile and nearly all of that traffic was coming from social media, so a familiar interface was welcomed. To ensure our core concepts of grappling and accessible were met, the first thing shown on the site was the most recent content piece posted. This long form video content was already being marketed in pieces, so the full thing would be exactly what they're looking for on their first visit.  

Directly below this was merch items to be sold. This allowed returning visitors to support the website and have it in view on every visit. 

Finally, we have all previous releases and posts that would interest visitors. This gives them more content to keep them on the site and binge.

### Version Two (growth)

In a digital age, the growth of any company comes from the community you've built around it. The hardest part isn't creating a solid product, but creating a connection to your customers and audience. With the exponential monthly growth in this audience, I wanted to further the connection and community I created. To do this I planned to showcase other artists within this community in the form of playlists. Every week I would take submissions from community members that visited the site and share new additions to the playlist on social media platforms.

#### Form Submissions
As mentioned above, for hosting I utilized netlify which, has built-in form submission on their platform. It didn't require much additional configuration from the standard HTML and CSS in creating a form, and it also included a spam-filter, which ended up being *VERY* necessary.

```
<form
        name="submissions"
        method="POST"
        netlify-honeypot="bot-field"
        data-netlify="true"
        action="/success"
      >
```

The only negative of this edition was I recieved too many submissions  . . . so many that netlify no longer let my site be hosted for free; as I quickly reached the free monthly limit of submissions in the first week.

#### Re-worked Navigation

With these newly added features, I now needed to have a way to make them easily **accessible.** The current navigation from Version one was . . . practically non-existent, as the focus was to have all content for users available on one page, but with growth comes change. The existing layout catered to replacing the existing cenetered social media icons with a nav bar.





### Version Three (Division)



