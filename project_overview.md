---
# This page uses Hydejack's `about` layout, which shows the primary author's picture and about text at the top.
# You can change it to the regular `page` layout if you want.
layout: page

# The title of the page.
title: Project Overview

# Write a short (~150 characters) description of each blog post.
# This description is used to preview the page on search engines, social media, etc.
description: >
  Project Overview

# You can show the description on the page by deleting this line:
hide_description: true

# Setting `menu` will generate an entry in the sidebar.
menu: true

order: 2
---
## Project Description
The Restroom Review (RR) website allows users to find and rate public restrooms near them. By browsing to the site on a mobile device, and allowing the site to use their location, they can see restrooms around them that have been reported and rated/reviewed by other users. Users can sort the restrooms by distance or rating, and they can also leave reviews or ratings themselves. If they've found a restroom that has not previously been reported, they can submit it to the site. 

Crowdsourced data powers the site - it is only as strong as it's user base. The Restroom Review project is an investigation into the power of crowdsourced data, including an exploration on what it takes to build a strong repository of data, as well as to understand any ethical concerns surrounding the use of crowdsourced data.

## Specific Aims
- Build a functional Restroom Review site that allows users to find and submit known public restrooms to the site database, as well as leave ratings or reviews for those restrooms.
- Build a user base of people who regularly access the site, in order to collect crowdsourced data that other users can utilize.
- Understand ethical concerns about crowdsourcing data in this fashion

## Project Site Requirements
- The RR site MUST allow a Visitor to authenticate themselves before leaving a review.
- The RR site MUST allow a Visitor to search for restrooms near a location.
- The RR site MUST allow a Visitor to share their location with the site and use it to search for restrooms.
- The RR site MUST NOT require a Visitor to share their location or any other personal information.
- The RR site MUST allow a Visitor to view a list of nearby restrooms.
- The RR site MUST allow a Visitor to sort the list of nearby restrooms by distance AND/OR by rating.
- The RR site MUST allow a Logged-in User to leave a review for a restroom.
- The RR site MUST allow a Logged-in User to leave a rating for a restroom.
- The RR site MUST allow a Logged-in User to leave a review OR rating anonymously.
- The RR site MUST allow a Logged-in User to delete the reviews they've written.
- The RR site SHOULD allow a Logged-in User to view the reviews they've written.
- The RR site SHOULD allow a Logged-in User to edit the reviews they've written.

## Use Cases
![](/assets/img/use-case-diagram.png)