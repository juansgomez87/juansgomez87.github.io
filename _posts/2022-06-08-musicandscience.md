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


### Pie charts

These pie charts should be read from inside to outside: firstly we have the proportion of participants that were assigned to the groups "center", "right", and "left". Then we have the models that were assigned to each one of the participants: *ACO*, *LYR*, *MIX*, and *RAND*. Finally, we have the proportion of music that was predicted to have high probability of being negatively valenced according to the personalized models. In this case, we aggregate the top 20 predictions and plot the proportion of music belonging to each type: FARC-songs, AUC-songs, and music without lyrics. 


<iframe
  src="{{ site.url }}/images/tests_music_and_science/test_agg.html"
  style="width:100%; height:600px;"
></iframe>

The following plot is more informative 
After the layer that shows the models, we show the anonymized user ids. Here it is possible to see that the *MIX* models from users 33 and 34 ("left") indeed captured that AUC-music ("right-wing") was negatively valenced. In the case of "right" users, we find that user 93 (with *ACO* model), user 103 (with *LYR* model), and user 26 (with *MIX* model) has high proportion of FARC-music ("left-wing").

<iframe
  src="{{ site.url }}/images/tests_music_and_science/test_full.html"
  style="width:100%; height:600px;"
></iframe>

Although the differences are not as discernible in general, we believe this to be problematic. 


