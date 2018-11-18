---
layout: home
title: Research
description: "Audio Signal Processing &amp; Deep Learning"
header-img: images/homepage.jpg
comments: false
modified: 2018-11-11
---

### Jazz Solo Recognition with Convolutional Neural Networks

This code contains a show case of the paper *"Jazz Solo Instrument Classification with Convolutional Neural Networks, Source Separation, and Transfer Learning"* that was accepted in the ISMIR 2018 conference. <br/>

The code contains wav examples and the trained ConvNets to plot segment- and clip-wise predictions of the instruments in the an audio mixture. <br/>

The model has been trained to recognize the following instruments: soprano saxophone (ss), alto saxophone (as), tenor saxophone (ts), clarinet (cl), trombone (tb), and trumpet (tp). <br/>
The audio contains 6 jazz solos:
- Ornette Coleman - Ramblin (as)
- Buddy DeFranco - Autumn Leaves (cl)
- John Coltrane - My Favorite Things (ss)
- Frank Rossolino - Moonlight in Vermont (tb)
- Lee Morgan - The Sidewinder (tp)
- Michael Brecker - African Skies (ts)

You can check out the code [here.](https://github.com/juansgomez87/jazz-show-case/)

You can read the paper [here.](http://ismir2018.ircam.fr/doc/pdfs/145_Paper.pdf)

An example of a real-time implementation using of the neural network can be seen in this video:

[![Real-Time Instrument Recognition](https://img.youtube.com/vi/KEcjxkJd0SQ/0.jpg)](https://www.youtube.com/watch?v=KEcjxkJd0SQ)

---
### Audio Object Localization and Recognition

This Media Project considers the task of creating an audio sound source localization and activity detection algorithm to be used on a robotic platform. The proposed real-time processing framework (written in Python) is able to create an internal representation of the sound objects in its surroundings and recognizes speech as a source of interest. The robotic platform will then take this information to move towards the source of interest.

Several active localization algorithms have been proposed in the literature to calculate the 3D position of a sound source, taking into account the time delay of arrival (TDOA). The implemented approach is based on the General Cross Correlation with Phase Transform (GCC-PHAT) method introduced by Knapp and the implementation of the [Multichannel BSS Locate by Lebarbenchon et al.](http://bass-db.gforge.inria.fr/bss_locate/) 

The localization algorithm using the MiniDSP UMA-8 microphone array can be seen in this video:

[![Audio Object Localization](https://img.youtube.com/vi/pNkb4o70zHs/0.jpg)](https://www.youtube.com/watch?v=pNkb4o70zHs)

The sound source activity detector is based on a system proposed by Rossi et al., where a variant of Mel-frequency Cepstrum Coefficients (MFCC) feature is used on support vector machine classification to solve real-time monophonic sound event classification.

The complete functioning system can be seen in this video:

[![Audio Object Localization and Recognition on a Robotic Platform](https://img.youtube.com/vi/4iSJTyEVjYc/0.jpg)](hhttps://www.youtube.com/watch?v=4iSJTyEVjYc)

---
### Time Reversal Room Impulse Response

Based on the paper by Zhung-Han Wu et al. *"A Time-Reversal Paradigm for Indoor Positioning System"*, this script uses PyAudio to playback an impulse through the speakers while recording simultaneously. The natural convolution of the impulse with the room acoustics results in obtaining the room impulse response. Following the paper, reproducing the time-reversed room impulse response will again make a natural convolution with the room, obtaining an impulse. The time and magnitude of this impulse varies with respect to the distance between receiver (microphone) and transmitter (speakers).

You can check the code out [here.](https://github.com/juansgomez87/time-reversed-rir/)


