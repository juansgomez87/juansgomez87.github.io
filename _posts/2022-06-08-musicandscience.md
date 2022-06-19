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


### Right-wing authoritarianism scale

Please indicate how strongly do you agree or disagree with the following statements (1 means strongly disagree and 5 means strongly agree).

|  Question |
|--------------|
|Our country needs a powerful leader, in order to destroy the radical and immoral currents prevailing in society today.|
|Our country needs free thinkers, who will have the courage to stand up against traditional ways, even if this upsets many people.|
|The ‘‘old-fashioned ways’’ and ‘‘old-fashioned values’’ still show the best way to live.|
|Our society would be better off if we showed tolerance and understanding for untraditional values and opinions."|
|God's laws about abortion, pornography and marriage must be strictly followed before it is too late, violations must be punished.|
|The society needs to show openness towards people thinking differently, rather than a strong leader, the world is not particularly evil or dangerous.|
|It would be best if newspapers were censored so that people would not be able to get hold of destructive and disgusting material.|
|Many good people challenge the state, criticize the church and ignore ‘‘the normal way of living’’.|
|Our forefathers ought to be honored more for the way they have built our society, at the same time we ought to put an end to those forces destroying it.|
|People ought to put less attention to the Bible and religion, instead they ought to develop their own moral standards.|
|There are many radical, immoral people trying to ruin things; the society ought to stop them.|
|It is better to accept bad literature than to censor it.|
|Facts show that we have to be harder against crime and sexual immorality, in order to uphold law and order.|
|The situation in the society of today would be improved if troublemakers were treated with reason and humanity.|
|If the society so wants, it is the duty of every true citizen to help eliminate the evil that poisons our country from within.|


### Social dominance orientation scale

Please indicate how strongly do you oppose or favor the following statements (1 means strongly oppose and 5 means strongly favor).

|  Question |
|--------------|
|An ideal society requires some groups to be on top and others to be on the bottom.|
|Some groups of people are simply inferior to other groups.|
|No one group should dominate in society.|
|Groups at the bottom are just as deserving as groups at the top.|
|Group equality should not be our primary goal.|
|It is unjust to try to make groups equal.|
|We should do what we can to equalize conditions for different groups.|
|We should work to give all groups an equal chance to succeed.|


### Colombian specific political questionnaire

Please indicate how strongly do you oppose or favor the following statements (1 means strongly oppose and 5 means strongly favor).

|  Question |
|--------------|
|We have to combat criminal organization by increasing the operative capabilities and presence of the public force.|
|We must develop a program of citizen cohabitation as a mechanism to prevent crime and solve conflicts.|
|The reasons for insecurity are: hunger, non-inclusion of young citizens, and the lack of compliance with the peace treaty.|
|We must strongly fight FARC dissidents that cheated us by taking advantage of the peace treaty to become strong and continue committing crimes.|
|We should qualify the ESMAD with classes on human rights, political and social aspects of the national reality.|
|It is necessary to dismantle the ESMAD and to transit to a new force which is oriented to peaceful and intelligent solution of conflicts.|
|We should generate conditions for greater investment in responsible mining/energy projects.|
|The transition between coal mining and oil to renewable energies is necessary, but should be accomplished gradually.|
|We should start the transition to clean and renewable energies now, leaving aside the extractivist logic of the oil industry.|

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

