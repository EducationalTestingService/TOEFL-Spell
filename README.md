# TOEFL-Spell
A dataset of Spelling Annotations for English language learner essays written for TOEFL exams.

This repository contains the TOEFL-Spel annotated data set. The data is described in the paper
*A Benchmark Corpus of English Misspellings and a Minimally-supervised Model for Spelling Correction*
 [(Flor, Fried & Rozovskaya, 2019)](https://www.aclweb.org/anthology).
 

The data set contains annotations of 6000+ spelling errors from
essays written by non-native speakers of English taking the TOEFL iBT test.

We based our data set on the publicly available ETS
Corpus of Non-Native Written English , a.k.a. TOEFL11.
TOEFL11 contains 12,100 essays from 11 first language backgrounds
We sampled 883 essays from that corpus and manually annotated them for spelling errors.

The supplied file contains tab-separated annotations for all the data.
Each annotation appears on a separate line.
The value of the *Filename* field matches the corresponding text file in the full TOEFL11 corpus.
The value in the *span* field gives the offset of the misspelling in the original text file.

In order to appreciate the annotations in full context of the original essay,
you will need to obtain the essays from the Linguistic Data Consortium (LDC Catalog Number: [LDC2014T06](https://catalog.ldc.upenn.edu/LDC2014T06)) and link them to the annotation via filenames and offset values.


Questions? Send email to mflor@ets.org


