---
layout: single
title: "About"
permalink: about
excerpt: "Bio."
toc: True
author_profile: True
---

I am a postdoc at [Télécom ParisTech](http://www.telecom-paristech.fr/eng){:target='_blank'} - [Université Paris-Saclay](https://www.universite-paris-saclay.fr/en){:target='_blank'} in the [Data, Intelligence and Graphs Team](https://dig.telecom-paristech.fr/blog/){:target='_blank'}.

I am the maintainer of [scikit-multiflow](https://scikit-multiflow.github.io/){:target='_blank'}.

## Research

My research interests are in the field of Machine Learning, including but not limited to:

- Learning from evolving data streams
- Data Imbalance
- Missing data imputation

Highlights from my time in academia and industry:

## Academia

Bachelor's Degree from _Puebla Institute of Technology_ (Mexico). I was Research Intern at the _Centre for Intelligent Machines_ in _McGill University_ (Canada). Research Assistant at the _National Institute of Astrophysics, Optics and Electronics_ (Mexico). Master’s Degree in Computer Science from the _Tokyo Institute of Technology_ (Japan), as fellow of the _Monbukagakusho Scholarship_ (Embassy Recommendation) from the Japanese Ministry of Education, Culture, Sports, Science and Technology. Research Assistant at the _Global Edge Institute_ (Japan). Lecturer at the _University of Queretaro_ (Mexico) in the Computer Science Department. PhD Degree in Computer Science from the Université Paris-Saclay -- Télécom-ParisTech (France).

## Industry

Tech Lead at _General Electric Aviation_ developing on-board software for Aircraft and Engine Prognostics; working in the development of GE's Brilliant Machines, part of the IoT and GE's approach to Industrial Big Data.

## Timeline

<style type="text/css">
  .timeline-logo   { float:left;
             vertical-align: middle;
             margin-right: 10px; }

  .timeline-text { vertical-align: middle;
            display: table-cell; }
</style>

<div>
    {% assign events = site.events | sort: 'date' %}
    {% for event in site.events reversed %}
    {% assign date = event.date | date: '%Y/%m' %}
    {% assign enddate = event.enddate | date: '%Y/%m' %}
    <big>{{ event.date | date: '%Y/%m' }}
    {% if event.enddate != blank %}
        {% if date < enddate %} - {{ event.enddate | date: '%Y/%m' }}
        {% endif %}
    {% else %} - 
    {% endif %}
    </big>
    <div>
        <img class="timeline-logo" src="{{site.baseurl}}{{ event.image }}" width="80" height="80">
        <span class="timleline-text"><small>{{ event.content }}</small></span>
    </div>
    <br><br>
    {% endfor %}
</div>