# Automatic Dubbing
TL;DR: this repo documents progress in automatic dubbing [science](#automatic-dubbing-science), 
[applications](#automatic-dubbing-applications), and [related](#automatic-dubbing-related) topics.


## Introduction
Briefly automatic dubbing (AD) is a task of reconstructing an audiovisual content using artificially synthesized 
audio and/or video, for language(s) different from the original production. For instance, AD can be used for dubbing 
the movie [Interstellar](https://www.imdb.com/title/tt0816692/) from the production language (English) into 
other languages like Italian, Chinese, or Amharic. This is what makes AD cool! as one of the most exciting 
applications of ML/AI. However, the science behind AD is still evolving. In an effort to track progress in AD, 
this repo documents scientific literature, tools, and other relevant materials.


In practice, AD works by machine translating the production language speech (_source_) into the new dubbing 
language (_target_), followed by prosodic alignment of target and source scripts, synthesizing target speech, 
and finally generation of the dubbed video. In AD, audiovisual coherence is indispensable, as no one enjoys the 
experience of watching a show/movie with timing mismatch between the visual and audio stream  - [lip-sync error](https://en.wikipedia.org/wiki/Lip_sync).


*Note*
* Organization - notes in this repo has three main sections: science, application, and related topics.
* Materials - are directly or indirectly utilized for an AD or related use cases such as automatic voice-over, lip-syncing, or sub-titling.
* Missing item - if you know a paper, and don’t see it documented here, please do a PR or send the info 
over [email](surawinfo@gmail.com), Thanks!



---
## Automatic Dubbing Science
Science is organized after an [AD pipeline](https://www.amazon.science/publications/from-speech-to-speech-translation-to-automatic-dubbing), 
covering an Automatic Speech Recognition (SR), Machine Translation (MT), Prosodic Alignment (PA), and 
Text-to-Speech (TS) modules.


#### Speech Recognition: SR


#### Machine Translation: MT
[The Two Shades of Dubbing in Neural Machine Translation, COLING, 2022](https://aclanthology.org/2020.coling-main.382.pdf)
- Proposes to apply relaxed translation length constraint for off-screen (_i.e when a character lip is not visible on screen_) 
   AD, to ultimately minimize the impact on translation quality.


#### Prosodic Alignment: PA


#### Text to Speech: TS


#### Face/Lip Detection/Generation: LipSync


---
## Automatic Dubbing Applications
A cascaded and an End-to-end approaches are considered as an application of AD. Cascaded AD is a pipeline of 
independently trained and managed models such as ST, MT, PA, and TS. In contrast, End-to-end AD utilizes a single model 
to achieve the tasks in cascaded AD.  

#### Cascaded Automatic Dubbing

[From Speech-to-Speech Translation to Automatic Dubbing](https://aclanthology.org/2020.iwslt-1.31.pdf), IWSLT, 2020
- Proposes to leverage robust SR, MT that controls the output length, PA to align source speech segments with MT outputs, 
and TS with a feature to adjust the duration of speech segments, to create an AD experience.  

[Face-Dubbing++: Lip-Synchronous, Voice Preserving Translation of Videos](https://arxiv.org/pdf/2206.04523.pdf), arXiv, 2022
- Focuses on synthetic lip/face generation for a lip-sync AD, using SR with word emphases detection, MT with emphases 
transfer capability, and TS with a voice conversion module.  

#### End-to-End Automatic Dubbing


---
## Automatic Dubbing Related
Section is dedicated to document materials such as books, articles, tools, and relevant analysis on AD.
