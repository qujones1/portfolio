---
title: Gatsby Tiktok Pixel plugin
date: 2022/4/14
description: Desciprtion of my Tiktok Pixel plugin Development.
tag: web development
author: Quentin Jones
---

# Gatsby Tiktok Pixel Plugin

## Introduction

If you're not heavily involved in digital marketing, you may be unfamiliar with the tiktok pixel.
I won't go over the technology heavily here, but to briefly describe: Pixels sit on your site almost like a digital shop keeper and collect data on what actions your sites visitors do and report it to an external source. Facebook, Snapchat, Google, and *Tiktok* all have their own.
They provide very easy integrations with Shopify, Wix, etc. to ensure you can utilize this function for their ad services. This allows you to create custom audiences based on your visitors, or run ads to target conversions for specific actions on your site.
And, if you don't use the premade site services, a script is provided to be added over the <head> tag in your html and CSS. This is where a problem with my site was introduced, as react does not let you embed runnable script directly and in order to have accurate data, I had to track page changes and this could not be done if the script was ran on page load.
  
## The Plugin
  
  The script needed to be run on every route change and page load, to accomplish this I utilized Gatsby's [onRouteChange](https://www.gatsbyjs.com/docs/reference/config-files/gatsby-browser/#onRouteUpdate) API.
  
  

This ensures on every page and page change a **ViewContent** action was tracked.
Now we just need to run the script on each render.
  

This also adds the capability of adding multiple pixels quickly by simply updating the Gatsby-config.js file with multiple pixelId Options:

