---
# Posts need to have the `post` layout
layout: post

# The title of your post
title: Initial Architecture and Browsing the Literature

# (Optional) Write a short (~150 characters) description of each blog post.
# This description is used to preview the page on search engines, social media, etc.
# description: >
#   Description goes here

# (Optional) Link to an image that represents your blog post.
# The aspect ratio should be ~16:9.
image: /assets/img/default.jpg

# You can hide the description and/or image from the output
# (only visible to search engines) by setting:
# hide_description: true
# hide_image: true

# (Optional) Each post can have zero or more categories, and zero or more tags.
# The difference is that categories will be part of the URL, while tags will not.
# E.g. the URL of this post is <site.baseurl>/hydejack/2017/11/23/example-content/
categories: [project]
tags: [project, update]
# If you want a category or tag to have its own page,
# check out `_featured_categories` and `_featured_tags` respectively.
---

I began thinking about the architecture of the Restroom Review site (which, by the way, I'm still trying to think of a better name for). My experience with working on full-stack development is leading me towards using Microsoft's (cross-platform) dotnet core to create a REST API backed by a PostgreSQL database, and developing a React front end application to make up the front end. 

I'm wondering if I want to require users to authenticate. I wouldn't do my own authentication solution - I'd probably use the open source Firebase for identty management so users could login with their Google accounts. But I could also just have the site be completely open - and just put a reCAPTCHA on the forms to avoid bot spam. The only trouble with that is that if I want the scope to be limited initially to the Northeastern campus and surrounding area, having no authentication leaves the site open to pretty much anyone from anywhere. 

I also started investigating some literature about crowdsourcing data. There has been no shortage on papers (and this just using Google Scholar for now) ranging from articles on ethics to recommendations about how to de-noise and filter raw crowdsourced data. I have had some difficulties trying to find ethical implications of using crowdsourced data for a site like mine, as opposed to ethical concerns when using a crowdsourced data platform to collect survey data. I think the second article I looked at ["Internet-based crowdsourcing and research ethics"](/literature/#internet-based-crowdsourcing-and-research-ethics) had some relevant ideas about the actual collection of data via crowdsourcing being an experiment itself. 

Next steps: I want to find some more articles on data collection techniques and best practices. I also want to pin down the exact REST API architecture, since I want to have that done by 2/02. For web hosting, GitHub student comes with credits for DigitalOcean for projects just like this one, so I think that will be a good resource. 

Oh and I want to come up with a better name for the site!
