---
layout: single
title: "About"
permalink: /about/
excerpt: "Bio."
toc: True
author_profile: True
---

I am a Ph.D. student at [Télécom ParisTech](http://www.telecom-paristech.fr/eng){:target='_blank'} - [Université Paris-Saclay](https://www.universite-paris-saclay.fr/en){:target='_blank'} in the [Data, Intelligence and Graphs Team](https://dig.telecom-paristech.fr/blog/){:target='_blank'}, under the supervision of [Talel Abdessalem](https://sites.google.com/view/talel-abdessalem){:target='_blank'} and [Albert Bifet](http://albertbifet.com/){:target='_blank'}.

I am the maintainer of [scikit-multiflow](https://scikit-multiflow.github.io/){:target='_blank'}.

## Academia

Bachelor's Degree from _Puebla Institute of Technology_ (Mexico). Research Intern at the _Centre for Intelligent Machines_ in _McGill University_ (Canada). Research Assistant at the _National Institute of Astrophysics, Optics and Electronics_ (Mexico). Master’s Degree in Computer Science from the _Tokyo Institute of Technology_ (Japan), as fellow of the _Monbukagakusho Scholarship_ (Embassy Recommendation) from the Japanese Ministry of Education, Culture, Sports, Science and Technology. Research Assistant at the _Global Edge Institute_ (Japan). Lecturer at the _University of Queretaro_ (Mexico) in the Computer Science Department for the master courses 'Pattern Recognition', 'Analysis of Algorithms', and 'Advanced Data Structures'.

## Industry
 Tech Lead at _General Electric Aviation_ developing on-board software for Aircraft and Engine's Prognostics; working in the development of GE’s Brilliant Machines, part of the IoT and GE’s approach to Industrial Big Data.

## Research

My research interests are in the field of Machine Learning with application on Big Data, including but not limited to:

- Stream Data Mining
- Risk Prediction
- Data Imbalance

## Timeline

<div class="container row">
    {% assign events = site.events | sort: 'date' %}
    {% for event in site.events reversed %}
    <div class="clearfix float-my-children">
        {% assign date = event.date | date: '%Y/%m' %}
        {% assign enddate = event.enddate | date: '%Y/%m' %}
        <big class="item-date">{{ event.date | date: '%Y/%m' }}
        {% if event.enddate != blank %}
            {% if date < enddate %} - {{ event.enddate | date: '%Y/%m' }}
            {% endif %}
        {% else %} - 
        {% endif %}</big>
        <div>
            <span>
                <img style="float:left" class="img-circle" src="{{site.baseurl}}{{ event.image }}" width="80" height="80"  hspace="20">
                {{ event.content }}
            </span>
        </div>
    </div>
    <br>
    {% endfor %}
    <div class="last-item">
        <i class="vertical-line"></i>
    </div>
</div>