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

You can check the code out [here.](https://github.com/juansgomez87/jazz-show-case/)

You can read the paper [here.](http://ismir2018.ircam.fr/doc/pdfs/145_Paper.pdf)

---
### Time Reversal Room Impulse Response

Based on the paper by Zhung-Han Wu et al. *"A Time-Reversal Paradigm for Indoor Positioning System"*, this script uses PyAudio to playback an impulse through the speakers while recording simultaneously. The natural convolution of the impulse with the room acoustics results in obtaining the room impulse response. Following the paper, reproducing the time-reversed room impulse response will again make a natural convolution with the room, obtaining an impulse. The time and magnitude of this impulse varies with respect to the distance between receiver (microphone) and transmitter (speakers).

You can check the code out [here.](https://github.com/juansgomez87/time-reversed-rir/)
