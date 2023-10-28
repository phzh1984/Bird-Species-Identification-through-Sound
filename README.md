# Bird-Species-Identification-through-Sound

This repository contains code and resources for a machine learning task aimed at identifying Eastern African bird species by their calls using passive acoustic monitoring (PAM). The task is crucial for monitoring and conserving avian biodiversity in the region and is in collaboration with NATURAL STATE, a Kenyan conservation organization.

The goal of the task is to develop computational solutions to process continuous audio data and accurately recognize Eastern African bird species based on their calls. The provided dataset consists of recordings made in Kenya, where participants must develop models to classify bird species in the audio recordings.

Dataset Description

train_audio: Contains short recordings of individual bird calls in the ogg format, sourced from xenocanto.org.

test_soundscapes: Directory populated with approximately 200 10-minute recordings in ogg audio format, used for scoring.

train_metadata.csv: Provides metadata including bird species codes, coordinates, author details, and file names for the training data.

Model Details

The model provided in this task is trained on Xeno-Canto recordings and produces output logits over more than 10k bird species. It also generates embedding vectors useful for various tasks. Note that the model's logit outputs are uncalibrated, which might affect interpretation in some cases.

Evaluation

Model quality is assessed by evaluating the classifier's performance on 5s segments of soundscapes from various datasets, using a peak-detector to associate ground-truth labels with each audio segment.




