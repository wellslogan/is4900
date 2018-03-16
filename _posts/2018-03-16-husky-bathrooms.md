---
layout: post
title: Husky Bathrooms
image: /assets/img/default.jpg
categories: [project]
tags: [project, update]
---

NEU RR Review has been rebranded, and now live at [huskybathrooms.com](https://www.huskybathrooms.com)! One pitfall I had with this was not remembering to update all of my Google API keys - there are different ones for Geocoding (mapping coordinates to an address, and vice-versa), Authentication, and reCAPTCHA - and they all recommend you lock down their use to a list of allowed domains. Mine were all locked down for `rr-neu-herokuapp.com` and `rr-neu-api.herokuapp.com` - which meant that the reCAPTCHA and location services didn't work for a while after I transfered the new domain over to the heroku app. Fortunately I caught the issue and was able to whitelist the new domain. 