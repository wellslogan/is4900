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
---

## Project Description
The goal of the Restroom Review (RR) site is to collect and provide crowdsourced data on public restrooms (initially limited to just those at Northeastern University in Boston, MA). The site will allow authenticated users (authenticated using Google as an identity provider - see [User Authentication](#user-authentication)) to identify and submit reviews for restrooms on campus. Unauthenticated users will be able to view reviews but must authenticate before they can leave reviews or ratings of their own.

A secondary goal of this project is an exploration into the feasibility of broadening the focus of the site to more than just the Northeastern University campus. Additionally, the ethics of using crowdsourced data in general will be explored. 

## Site Architecture
The RR site consists of two main components: the API and the front-end site.

### User Authentication
Authentication will be implemented using [Firebase](https://github.com/firebase/firebaseui-web){:target="_blank"} with Google as the primary identity provider.

### REST API
The API for the RR site will use dotnet core 2.0. Data storage will utilize a PostgreSQL database. A preliminary mapping of API endpoints is shown below:

| Route                              | HTTP Method             | POST Params                          |   
|:-----------------------------------|:------------------------|:-------------------------------------|
|`/rooms/`                           | GET                     | -                                    |   
|`/rooms/{id}`                       | GET                     | -                                    |   
|`/rooms/add`                        | GET                     | -                                    |   
|`/rooms/submit`                     | POST                    | [Room](#data-model-room)             |   
|`/rooms/{id}/reviews`               | GET                     | -                                    |   
|`/rooms/{id}/reviews`               | POST                    | [Review](#data-model-review)         |   

### Front-end Application
The actual RR website will be built with React.

### Data Models
#### <a id="data-model-room"></a>Room
<hr/>

| Field          | Type                            |
|:---------------|:--------------------------------|
| uid            | int                             |
| name           | string                          |
| description    | string                          |
| location       | Object { latitude , longitude } |

Schema:
```json
{
  "$schema": "http://json-schema.org/draft-06/schema#",
  "type": "object",
  "title": "Room",
  "uid": { "type": "number" },
  "name": { "type": "string" },
  "description": { "type": "string" },
  "location": {
    "type": "object",
    "latitude": { "type": "number" },
    "longitutde": { "type": "number" }
  }
}
```

Example:
```js
{
  uid: 123456789,
  name: "Snell Library 4th Floor Men's",
  descriptions: "",
  location: {
    latitude: "1.09897245",
    longitude: "0.94834234"
  }
}
```

#### <a id="data-model-review"></a>Review
<hr/>

| Field          | Type               |
|:---------------|:-------------------|
| uid            | int                |
| rating         | int                |
| description    | string             |
| roomuid        | int                |
| authoruid      | int                |

Schema: 
```json
{
  "$schema": "http://json-schema.org/draft-06/schema#",
  "title": "review",
  "type": "object",
  "uid": { "type": "number" },
  "rating": { "type": "number" },
  "description": { "type": "string" },
  "roomuid": { "type": "number" },
  "authoruid": { "type": "number" },
}
```

Example:
```js
{
  uid: 111111111,
  rating: 3,
  description: "Very clean",
  roomuid: 123456789,
  authoruid: 0
}
```

