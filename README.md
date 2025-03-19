# Project_Ego4D_NLQ_Benchmark
https://colab.research.google.com/drive/1RV0TctgCQRIphn3JHshZk4gBt60szV3q?usp=sharing

This project explores the use of natural language queries
for egocentric video understanding, leveraging the exten-
sive Ego4D dataset and its NLQ benchmark task. Our work
is divided into two phases: video moment localization and
the generation of textual answers based on the identified
moments. In the first phase, we address the NLQ task by
identifying the temporal segment of the video where a given
natural language query is answerable. We model this as a
regression problem using video span localizing networks:
VSLBase and its enhanced version, VSLNet. Both networks
learn cross-modal interactions between video and text fea-
tures through an attention-like mechanism, and they are
able to regress the span of the target moment. By incor-
porating the Query-Guided Highlighting (QGH) module,
VSLNet improves performance by focusing the search of the
target moment within the highlighted region.We trained and
validated this model using various combinations of power-
ful pre-trained models as fixed feature extractors for text
and visual features on the NLQ benchmark task. In the
second phase, we extend the project by extracting textual
answers from the identified target moments using a large
vision-language model, Video-LLaVA. This project demon-
strates progress towards developing an augmented reality
assistant capable of interpreting daily-life egocentric videos
and responding to queries about past activities.
