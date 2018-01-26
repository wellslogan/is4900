---
# This page uses Hydejack's `about` layout, which shows the primary author's picture and about text at the top.
# You can change it to the regular `page` layout if you want.
layout: page

# The title of the page.
title: Information

# Write a short (~150 characters) description of each blog post.
# This description is used to preview the page on search engines, social media, etc.
description: >
  Information about the project

# You can show the description on the page by deleting this line:
hide_description: true

# Setting `menu` will generate an entry in the sidebar.
menu: true

order: 3
---

## Project Description
The goal of the Restroom Review (RR) site is to collect and provide crowdsourced data on public restrooms (initially limited to just those at Northeastern University in Boston, MA). The site will allow authenticated users (authenticated using Google as an identity provider - see [User Authentication](#user-authentication)) to identify and submit reviews for restrooms on campus. Unauthenticated users will be able to view reviews but must authenticate before they can leave reviews or ratings of their own.

A secondary goal of this project is an exploration into the feasibility of broadening the focus of the site to more than just the Northeastern University campus. Additionally, the ethics of using crowdsourced data in general will be explored. 

## UML Class Diagram
![](/assets/img/uml.png)