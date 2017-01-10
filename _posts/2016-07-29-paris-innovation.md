---
layout: post
section-type: post
title: Paris Summer Innovation Fellowship
category: tech, data science
tags: [ 'activities', 'data science'  ]
---

<p style='text-align: justify;'>
I participated in the 2016 <a href="http://www.summerfellows.paris/"
target="_blank">Paris Summer Innovation Fellowship</a> in the following project
of the Data Science track.
</p>

### Optimizing restaurant health inspections through advanced analytics

<p style='text-align: justify;'>
The Ministry of Agriculture, Agri-food, and Forestry of France (Ministère de
l'Agriculture, de l'Agroalimentaire et de la Forêt) regularly inspects
businesses serving food to ensure restaurants and other food retail outlets are
following safe food handling procedures. Such task is bounded by time and human
resources, in other words, there is not enough time to inspect all restaurants
in one year and there are not enough inspectors to speed up the process.<br />
<br />
During 2015, 843 restaurants were inspected only in the Paris region. Each
inspected restaurant was awarded a note:<br />
<br />
A: Everything is correct [Best]<br />
B: Minor issues<br />
C: Major issues that need to be corrected<br />
D: Major issues were previously found and were not corrected [Worst]<br />
</p>

![Inspections 2015](/img/post_psif2016/inspection-notes.png)

<p style='text-align: justify;'>
Given this scenario, one way to optimize the use of resources for the restaurant
health inspections is by focusing on those restaurants with higher risk.
Since the number of inspectors is limited, it was proposed to make use of
information available in platforms like TripAdvisor, where user perform
'informal' reviews of restaurants, the assumption is that user reviews
potentially contain hints of health issues. TripAdvisor contains reviews for 8x
the number of restaurants inspected in 2015 in the Paris Region. In the
following image, blue dots correspond to inspected restaurants (Ministry of
Agriculture) and orange dots correspond to reviewed restaurants (TripAdvisor).
</p>

![Inspections and Reviews](/img/post_psif2016/inspections-reviews.png)

<img src="/img/post_psif2016/steps.png" border="none" />

![Model](/img/post_psif2016/predictions.png)

![High Risk](/img/post_psif2016/note-d.png)
