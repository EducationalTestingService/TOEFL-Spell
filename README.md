# TOEFL-Spell
A dataset of Spelling Annotations for English language learner essays written for TOEFL exams.

This repository contains the TOEFL-Spell annotated data set. The data is described in the paper
*A Benchmark Corpus of English Misspellings and a Minimally-supervised Model for Spelling Correction*
 [(Flor, Fried & Rozovskaya, 2019)](https://www.aclweb.org/anthology).
 

The TOEFL-Spell data set contains annotations of 6000+ spelling errors from
essays written by non-native speakers of English taking the TOEFL iBT test.

We based our data set on the publicly available ETS
Corpus of Non-Native Written English, a.k.a. TOEFL11,
which contains 12,100 essays from 11 first language backgrounds.
We sampled 883 essays from that corpus and manually annotated them for spelling errors.

We provide two files: FilesCounts.tsv and Annotations.tsv  (both have tab-separated values, first line is header). 
(There are now also FilesCounts.csv and Annotations.csv, that have the same data in csv format).

*FilesCounts.tsv* contains the names of annotated files (essays) and the count of spelling errros for each. Note that 35 essays had no spelling errors.

The file *Annotations.tsv* contains tab-separated annotations for all the data.
Each annotation appears on a separate line, like this:

Filename | OffsetSpan | Misspelling | Type | Correction
-------- | ---------- | ----------- | ---- | ----------
1004135 |	1186-1193	| beacuse |	M	| because

The value of the *Filename* field matches the corresponding text file in the full TOEFL11 corpus.
The value in the *span* field gives the offset of the misspelling in the original text file.

In order to appreciate the annotations in full context of the original essay (or to run your own experiments),
you will need to obtain the essays from the Linguistic Data Consortium (LDC Catalog Number: [LDC2014T06](https://catalog.ldc.upenn.edu/LDC2014T06)) and link them to the annotation via filenames and offset values.

### A note on 'types' of misspellings ###

The article mentions 6121 misspelings, where each is a single token nonword.
Those are marked as type M in the annotation.
The annotation file has 112 additional misspellings, with other type names (M2,MWM,MWM2), which were marked for addiitoanl research.
Only type M misspellings were used in system evaluations reported in the paper.

Questions? Send email to mflor@ets.org


