---
layout: post
title: Audio Object Localization and Recognition
description: 
author: Juan Gómez
create: 2018-11-06
image:
    feature: abstract-10.jpg
categories: [Research]
tags: [localization, recognition, real-time, audio signal, dsp, gcc, roomba robot]
---

This Media Project considers the task of creating an audio sound source localization and activity detection algorithm to be used on a robotic platform. The proposed real-time processing framework (written in Python) is able to create an internal representation of the sound objects in its surroundings and recognizes speech as a source of interest. The robotic platform will then take this information to move towards the source of interest.

Several active localization algorithms have been proposed in the literature to calculate the 3D position of a sound source, taking into account the time delay of arrival (TDOA). The implemented approach is based on the General Cross Correlation with Phase Transform (GCC-PHAT) method introduced by Knapp and the implementation of the [Multichannel BSS Locate by Lebarbenchon et al.](http://bass-db.gforge.inria.fr/bss_locate/) 

The localization algorithm using the MiniDSP UMA-8 microphone array can be seen in this video:

[![Audio Object Localization](https://img.youtube.com/vi/pNkb4o70zHs/0.jpg)](https://www.youtube.com/watch?v=pNkb4o70zHs)

The sound source activity detector is based on a system proposed by Rossi et al., where a variant of Mel-frequency Cepstrum Coefficients (MFCC) feature is used on support vector machine classification to solve real-time monophonic sound event classification.

The complete functioning system can be seen in this video:

[![Audio Object Localization and Recognition on a Robotic Platform](https://img.youtube.com/vi/4iSJTyEVjYc/0.jpg)](hhttps://www.youtube.com/watch?v=4iSJTyEVjYc)