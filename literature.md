---
# This page uses Hydejack's `about` layout, which shows the primary author's picture and about text at the top.
# You can change it to the regular `page` layout if you want.
layout: page

# The title of the page.
title: Literature

# Write a short (~150 characters) description of each blog post.
# This description is used to preview the page on search engines, social media, etc.
description: >
  Relevant literature to my project

# You can show the description on the page by deleting this line:
hide_description: true

# Setting `menu` will generate an entry in the sidebar.
menu: true

order: 4
---

Relevant literature related to the collection and usage of crowdsourced data.

## Contents
- [On the Ethics of Crowdsourced Resource](#on-the-ethics-of-crowdsourced-research)
- [Internet-based crowdsourcing and research ethics](#internet-based-crowdsourcing-and-research-ethics)
- [Maximizing Benefits from Crowdsourced Data](#maximizing-benefits-from-crowdsourced-data)
- [Comparing the Quality of Crowdsourced Data Contributed by Expert and Non-Experts](#comparing-the-quality-of-crowdsourced-data-contributed-by-expert-and-non-experts)
- [Lessons learned from the design, implementation, and management of a smartphone-based crowdsourcing system](#lessons-learned-from-the-design-implementation-and-management-of-a-smartphone-based-crowdsourcing-system)
- [Eliminating Spammers and Ranking Annotators for Crowdsourced Labeling Tasks](#eliminating-spammers-and-ranking-annotators-for-crowdsourced-labeling-tasks)


### On the Ethics of Crowdsourced Research
**[Vanessa Williams, Political Science & Politics, 2016](https://www.cambridge.org/core/journals/ps-political-science-and-politics/article/on-the-ethics-of-crowdsourced-research/B1BDFB1111B416DD0B71540CD6E7D94F){:target="_blank"}**

This source explores the ethics of the crowdsourcing platform Mechanical Turk (MTurk), an Amazon offering which allows users to complete simple tasks in exchange for a small amount of money per completion. The tasks in question can range from answering a market research question to more advanced tasks like transcribing audio or performing manual OCR (optical character recognition). 

Williamson notes that since 2009 there has been a sharp uptick in articles on the digital library JSTOR which contain data sourced from MTurk, and that this trend seems to exist across different digital libraries as well. She does point out that while this data is considered "often more representative of the US population than in-person convenience samples" (qtd. in Williamson, 77), it might not be so simple - "About 80% of tasks on MTurk are completed by about 20% of participants, who spend more than 15 hours a week working on MTurk" (77). This means that there might be different ethical concerns when relying on the data on MTurk users - since such a significant portion of data is gathered from users who view the platform as essentially a part time job.

Williamson conducted interviews with 49 MTurk users who responded to an initial question on MTurk itself. Many of the folks she spoke to "[reported] using the service as a major source of income" (78). The end results of her research - there are significant ethical concerns of using crowdsourced data from a source like Mechanical Turk, where many users simply use the site as a source of income instead of a more broad voluntary survey platform. 

[Contents &#x21a9;&#xfe0e;](#contents)

### Internet-based crowdsourcing and research ethics 
**[Mark A. Graber and Abraham Graber, Journal of Medical Ethics, 2013](http://dx.doi.org/10.1136/medethics-2012-100798){:target="_blank"}**

This article (referenced in the above article ["On the Ethics of Crowdsourced Research"](#on-the-ethics-of-crowdsourced-research)) investigates the ethics of crowdsourcing data while looking at the Foldit project, which has contributors play a video game-like piece of software where the goal is to solve various protein folding problems, in order to help develop computer algorithms to do the same. The authors call this type of game a "greme," referring to a combination of game and research tool. 

The key point of this paper is that since the method by which crowdsourced data is collected is essentially a video game, there may be mechanisms at play that take advantage of the users by preying on an existing factor such as internet addiction - or that may simply cause an addiction to the "greme" itself. The authors do not conclude that such mechanisms are definitely involved in the collection of data, only that there is a possibility of them being involved. 

Another question raised in the paper is whether the players of the "greme" - the folks who are providing the crucial data to the project - should be considered human subjects. The authors' argument is that because it is impossible to know whether a specific "greme" will have meaningful results ahead of creating it and collecting data, the particpants and contributors are essentially the subjects of an initial expirement - which means that they should be subject to an IRB. 

The final conclusion of the authors is that the contributors of crowdsourced data is situations such as Foldit might in fact be subject to manipulation, making them human subjects, and making it so that in order to avoid any ethical breaches, IRB review must be required. 

[Contents &#x21a9;&#xfe0e;](#contents)

### Maximizing Benefits from Crowdsourced Data
**[Geoffrey Barbier, Reza Zafarani et al, Computational and Mathematical Organization Theory, 2012](https://link.springer.com/article/10.1007/s10588-012-9121-2){:target="_blank"}**

In this paper, crowdsourced data is typically not in a form that is immediately useful - take for example the kind of "data" you would get from a site like Yahoo Answers, which is one example they use, or Stack Overflow. Although this data is technically crowdsourced, there are still significant steps that need to be taken in order to get this data into a form that can be analyzed by software. The authors bring up four steps in processing the raw data - trust assessment (the trustworthiness of the data, considering the crowdsourcing platform), stop-word removal (removing "useless" words like "to" or "the"), vectorization (putting the data in a vector-tabular format), and feature extraction (converting the vector-tabular format to just tabular format). 

The authors also look at data mining that uses crowdsourced data to power machine learning - where humans perform work analyzing data in order to better train a computer algorithm to do the same, by validating computer-driven results with human results. An example brought up here is the original CAPTCHA, where in additional to providing web forms with protection against computer submissions also assisted machine learning algorithms in the detection of human handwriting.

Finally the authors of the paper talk about some of the challenges of crowdsourced data in general - filtering noise and dealing with junk or intentionally bogus information. They bring up a case of crowdsourcing relief efforts or crisis response, where after the initial processing is done on the data and it's in a somewhat usable form, there may still be areas where a human expert (say, on a particular region) would need to be brought in for further analysis. The bottom line - some denoising techniques are relatively easy, and apply to pretty much any raw data. But even once the data has been processed in this way, it may be necessary for more sophisticated techniques to be employed, techniques which require human analysis. 

[Contents &#x21a9;&#xfe0e;](#contents)

### Comparing the Quality of Crowdsourced Data Contributed by Expert and Non-Experts
**[Linda See, Alexis Comber et al, Public Library of Science (PLOS), 2013](http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0069958){:target="_blank"}**

This study takes a look at the quality of crowdsourced data used to determine human impacts on land cover, comparing between experts and non-experts. The study involved two measures, the degree of the human impact on a certain land area, and the type of land cover (e.g. shrub cover, tree cover, etc). 

The authors found that when it comes to determining whether there has been a discernible human impact on a land area, the level of expertise does not make a significant difference. However, when it comes to determining the type of land cover, experts performed significantly better than their non-expert counterparts. 

The authors suggest that a potential way to make bridge the gap would be to offer additional training and assistance for the non-experts in determining the type of land cover. This has implications for my project I think, since although determining land cover is a more complex and skilled task, it may be advantageous to provide some key factors that a restroom should have that might influence the rating. Rather than simply being a very open-ended "how would you rate this restroom," maybe ask reviewers to consider different factors such as "how would you rate the cleanliness of the restroom, scale of 1 to 10". 


[Contents &#x21a9;&#xfe0e;](#contents)

### Lessons learned from the design, implementation, and management of a smartphone-based crowdsourcing system
**[Andriano Faggiani, Enrico Gregori et al, ACM, 2013](https://dl.acm.org/citation.cfm?id=2536717){:target="_blank"}**

In this papers the authors built an app called Portolan, which uses crowdsourced information from its users to build and measure the internet and other networks in order to build internet topologies. The authors step through the creation of this app and talk about the lessons they learned from sourcing data from the crowd. 

Some of the issues they discuss apply more to the specific application architecture they decided to go with - for example, an issue with their Android app where users weren't updating to the latest versions. This isn't really applicable to a website, since a website is non-versioned and cross-platform by nature. 

A few other things the authors touch on are applicable, however. They mention the need for a solid database backbone from the beginning, since with their project they quickly had to scale their database-end in order to meet the needs of their growing user base. There are more algorithms in place for the Portolan app that make this more difficult then say, a review website, but the advice is still solid.

Another issue they ran into was motivating users to actually use their app. Since the end result of the user's direct interaction with the app was not that motivating (since it was only looking at the bigger picture that would cause the network topologies to come together), they added some basic network tools that the users could use while also providing the crucial crowdsourced data to the app. Motivation is something that I am somewhat concerned about, although a review website has the benefit of being a source of information for users, so they at least have a reason to visit the site. 

[Contents &#x21a9;&#xfe0e;](#contents)

### Eliminating Spammers and Ranking Annotators for Crowdsourced Labeling Tasks
**[Vikas Raykar and Shipeng Yu, Journal of Machine Learning Research, 2012](https://dl.acm.org/citation.cfm?id=2188401){:target="_blank"}**

[Contents &#x21a9;&#xfe0e;](#contents)
