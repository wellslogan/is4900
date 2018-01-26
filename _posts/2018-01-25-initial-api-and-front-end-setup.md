---
# Posts need to have the `post` layout
layout: post

# The title of your post
title: Setup of API and Front End Projects for the Site

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
Yesterday I got put together two projects for the [API](https://github.com/wellslogan/RR-NEU-API){:target="_blank"} and 
[site](https://github.com/wellslogan/RR-NEU-Site){:target="_blank"}, and now they are up on Github. For the back end, I'm using .NET Core 2.0 backed by a PostgreSQL database - getting the DB up and running still on the agenda. I added a few simple routes for the different rooms and reviews, as well as some models following the design in my [class diagram on the information page](/information/#uml-class-diagram).  

The front end took some more effort to put together, even though I do have prior experience with React applications. I'm using a custom webpack config so I can get control over the Typescript compilation and SASS bundling. Didn't add uch functionality onto the actual React side of things besides configuring React Router with a few simple routes - I want to get the API mostly functional and then I can start implementing some actual front end services that hit the REST methods in the API. 