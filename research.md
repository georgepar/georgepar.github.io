---
layout: page
permalink: /research/
title: Research
pubs:

    - title:   "Speech data augmentation"
      author:  "Georgios Paraskevopoulos, Evangelia Chatziagapi, Theodoros Giannakopoulos, Alexandros Potamianos, Shrikanth Narayanan"
      journal: "US Patent App. 16/852,793"
      year:    "2020"

    - title:   "Deep hierarchical fusion for machine intelligence applications"
      author:  "Efthymis Georgiou, Georgios Paraskevopoulos, James Gibson, Alexandros Potamianos, Shrikanth Narayanan"
      journal: "US Patent App. 16/852,793"
      year:    "2020"

    - title:   "Multimodal and multiresolution speech recognition with transformers"
      author:  "Georgios Paraskevopoulos, Srinivas Parthasarathy, Aparna Khare, Shiva Sundaram"
      journal: "Proceedings of the 58th Annual Meeting of the Association for Computational Linguistics"
      year:    "2020"

    - title:   "Affective Conditioning on Hierarchical Networks applied to Depression Detection from Transcribed Clinical Interviews"
      author:  "Danai Xezonaki, Georgios Paraskevopoulos, Alexandros Potamianos, Shrikanth Narayanan"
      journal: "Interspeech"
      year:    "2020"

    - title:   "Data Augmentation Using GANs for Speech Emotion Recognition"
      author:  "Aggelina Chatziagapi, Georgios Paraskevopoulos, Dimitris Sgouropoulos, Georgios Pantazopoulos, Malvina Nikandrou, Theodoros Giannakopoulos, Athanasios Katsamanis, Alexandros Potamianos, Shrikanth Narayanan"
      journal: "Interspeech"
      year:    "2019"

    - title:   "Real-time arm gesture recognition using 3D skeleton joint data"
      author:  "Georgios Paraskevopoulos, Evaggelos Spyrou, Dimitrios Sgouropoulos, Theodoros Giannakopoulos, Phivos Mylonas"
      journal: "Algorithms"
      year:    "2019"

    - title: "Unsupervised Low-Rank Representations for Speech Emotion Recognition"
      author: "Georgios Paraskevopoulos, Efthymios Tzinis, Nikolaos Ellinas, Theodoros Giannakopoulos, Alexandros Potamianos"
      journal: "Interspeech"
      year: "2019"

    - title: "Integrating Recurrence Dynamics for Speech Emotion Recognition"
      author: "Efthymios Tzinis, Georgios Paraskevopoulos, Christos Baziotis, Alexandros Potamianos"
      journal: "Interspeech"
      year: "2018"

    - title: "Pattern search multidimensional scaling"
      author: "Georgios Paraskevopoulos, Efthymios Tzinis, Emmanouil-Vasileios Vlatakis-Gkaragkounis, Alexandros Potamianos"
      journal: "ArXiv"
      year: "2018"

    - title: "Ntua-slp at semeval-2018 task 3: Tracking ironic tweets using ensembles of word and character level attentive rnns"
      author: "Christos Baziotis, Nikos Athanasiou, Pinelopi Papalampidi, Athanasia Kolovou, Georgios Paraskevopoulos, Nikolaos Ellinas, Alexandros Potamianos"
      journal: "Proceedings of The 12th International Workshop on Semantic Evaluation"
      year: "2018"

    - title: "Ntua-slp at semeval-2018 task 1: Predicting affective content in tweets with deep attentive rnns and transfer learning"
      author: "Christos Baziotis, Nikos Athanasiou, Alexandra Chronopoulou, Athanasia Kolovou, Georgios Paraskevopoulos, Nikolaos Ellinas, Shrikanth Narayanan, Alexandros Potamianos"
      journal: "Proceedings of The 12th International Workshop on Semantic Evaluation"
      year: "2018"

    - title: "Ntua-slp at semeval-2018 task 2: Predicting emojis using rnns with context-aware attention"
      author: "Christos Baziotis, Nikos Athanasiou, Georgios Paraskevopoulos, Nikolaos Ellinas, Athanasia Kolovou, Alexandros Potamianos"
      journal: "Proceedings of The 12th International Workshop on Semantic Evaluation"
      year: "2018"

    - title: "Sensory-Aware Multimodal Fusion for Word Semantic Similarity Estimation"
      author: "Georgios Paraskevopoulos, Giannis Karamanolakis, Elias Iosif, Aggelos Pikrakis, Alexandros Potamianos"
      journal: "MultiLearn2017: Multimodal Processing, Modelingand Learning for Human-Computer/Robot Interaction Workshop"
      year: "2017"

    - title: "A real-time approach for gesture recognition using the Kinect sensor"
      author: "Georgios Paraskevopoulos, Evaggelos Spyrou, Dimitrios Sgouropoulos"
      journal: "Proceedings of the 9th Hellenic Conference on Artificial Intelligence"
      year: "2016"
---

## Publications (peer reviewed)

{% assign thumbnail="left" %}

{% for pub in page.pubs %}
{% if pub.image %}
{% include image.html url=pub.image caption="" height="100px" align=thumbnail %}
{% endif %}
[**{{pub.title}}**]({% if pub.internal %}{{pub.url | prepend: site.baseurl}}{% else %}{{pub.url}}{% endif %})<br />
{{pub.author}}<br />
*{{pub.journal}}*
{% if pub.note %} *({{pub.note}})*
{% endif %} *{{pub.year}}* {% if pub.doi %}[[doi]({{pub.doi}})]{% endif %}
{% if pub.media %}<br />Media: {% for article in pub.media %}[[{{article.name}}]({{article.url}})]{% endfor %}{% endif %}

{% endfor %}
