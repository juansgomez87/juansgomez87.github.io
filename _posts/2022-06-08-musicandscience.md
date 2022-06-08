---
layout: post
title: "Polarization through Colombian not-so-popular music and algorithms: appraisal guided musically induced emotions"
description: "Initial tests to visualize model results"
excerpt: "Initial tests"
author: Juan Gómez
create: 2021-06-08
image:
    feature: abstract-10.jpg
categories: [ideas]
tags: [personalization, colombian music]
---

## Polarization through Colombian not-so-popular music and algorithms: appraisal guided musically induced emotions


So far, we have 52 participants with full data out of 194. 

### Test 0

Using RWA to separate user groups and quantiles: left (RWA_score < 0.25), center (0.25 <= RWA_score <= 0.75), right (RWA_score > 0.75). 
We plot the proportion of top 20 songs with highest Q2 probability (Q2 quadrant: high arousal, negative valence). 


<iframe
  src="{{ site.url }}/images/tests_music_and_science/test_0.html"
  style="width:100%; height:600px;"
></iframe>


### Test 1
We do not consider music that has no lyrics in the top songs. 
This important because it is likely that music with no lyrics have a high probability of belonging to Q2, but this music is not interesting for our tests. 
Using RWA to separate user groups and quantiles: left (RWA_score < 0.25), center (0.25 <= RWA_score <= 0.75), right (RWA_score > 0.75). 
We plot the proportion of top 20 songs with highest Q2 probability (Q2 quadrant: high arousal, negative valence). 

<iframe
  src="{{ site.url }}/images/tests_music_and_science/test_1.html"
  style="width:100%; height:600px;"
></iframe>

"Right-leaning" users show more proportion of FARC music belonging to Q2, and "left-leaning" users show more proportion of AUC music belonging to Q2. However, this is not the same for every type of model and user. 

### Test 2

The proportion of "center" users is likely to be too high. We change the selection bounds to have very few "center" users.
Using RWA to separate user groups and quantiles: left (RWA_score < 0.35), center (0.35 <= RWA_score <= 0.65), right (RWA_score > 0.65). 
We plot the proportion of top 20 songs with highest Q2 probability (Q2 quadrant: high arousal, negative valence). 
We do not consider music that has no lyrics in the top songs. 

<iframe
  src="{{ site.url }}/images/tests_music_and_science/test_2.html"
  style="width:100%; height:600px;"
></iframe>

**Still we need to check how to make the user selection for each group**.

### Test 3

We test the predictions **only on valence**. The output probabilities of quadrants 1 and 4 belong to positive valence, and the ones from quadrants 2 and 3 belong to negative valence. 
We sort the output predictions acording to negative valence. 
Using RWA to separate user groups and quantiles: left (RWA_score < 0.35), center (0.35 <= RWA_score <= 0.65), right (RWA_score > 0.65). 
We plot the proportion of top 20 songs with highest negative valence probability. 
We do not consider music that has no lyrics in the top songs. 

<iframe
  src="{{ site.url }}/images/tests_music_and_science/test_3.html"
  style="width:100%; height:600px;"
></iframe>

Here we start to see a trend: "center" users show similar proportions, "right-leaning" users have higher proportions for FARC music (in red), and "left-leaning" users have higher proportions for AUC music (in blue). However, this trend is not general to all and does not maintain through models. 

### Test 4

We only consider participants to belong from "right" or "left":

<iframe
  src="{{ site.url }}/images/tests_music_and_science/test_4.html"
  style="width:100%; height:600px;"
></iframe>


