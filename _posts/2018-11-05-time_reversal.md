---
layout: post
title: Time Reversal Room Impulse Response
description: 
author: Juan Gómez
create: 2018-11-05
image:
    feature: abstract-10.jpg
categories: [Research]
tags: [impulse response, time reversal, pyaudio, acoustics]
---

Based on the paper by Zhung-Han Wu et al. *"A Time-Reversal Paradigm for Indoor Positioning System"*, this script uses PyAudio to playback an impulse through the speakers while recording simultaneously. The natural convolution of the impulse with the room acoustics results in obtaining the room impulse response. Following the paper, reproducing the time-reversed room impulse response will again make a natural convolution with the room, obtaining an impulse. The time and magnitude of this impulse varies with respect to the distance between receiver (microphone) and transmitter (speakers).

You can check the code out [here.](https://github.com/juansgomez87/time-reversed-rir/)