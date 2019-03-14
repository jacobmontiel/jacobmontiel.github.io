---
layout: single
title: IEEE BigData 2018
toc: False
author_profile: True
category: ['research']
tags: [ 'research', 'machine learning', 'stream learning', 'evolving data streams' ]
---

I am attending the [2018 IEEE International Conference on Big Data](http://cci.drexel.edu/bigdata/bigdata2018/) in Settle, USA, to present  our paper

**[Learning Fast and Slow: A Unified Batch/Stream Framework.](https://ieeexplore.ieee.org/document/8622222)**.

**Abstract:**
Data ubiquity highlights the need of efficient and adaptable data-driven solutions. In this paper, we present FAST AND SLOW LEARNING (FSL), a novel unified framework that sheds light on the symbiosis between batch and stream learning. FSL works by employing Fast (stream) and Slow (batch) Learners, emulating the mechanisms used by humans to make decisions. We showcase the applicability of FSL on the task of classification by introducing the FAST AND SLOW CLASSIFIER (FSC). A Fast Learner provides predictions on the spot, continuously updating its model and adapting to changes in the data. On the other hand, the Slow Learner provides predictions considering a wider spectrum of seen data, requiring more time and data to create complex models. Once that enough data has been collected, FSC trains the Slow Learner and starts tracking the performance of both learners. A drift detection mechanism triggers the creation of new Slow models when the current Slow model becomes obsolete. FSC selects between Fast and Slow Learners according to their performance on new incoming data. Test results on real and synthetic data show that FSC effectively drives the positive interaction of stream and batch models for learning from evolving data streams.
