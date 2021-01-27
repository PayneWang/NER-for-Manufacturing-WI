# NER-for-Manufacturing-WI

This repository contains a named entity recognition (NER) corpus for Chinese manufacturing work instruction (WI).

## Contributer
- Peiyan Wang

## Overview
This corpus contains 709 fabricating WI sentences,  774 assembly WI sentences,  and total 427,656 characters.  Fourteen types of entities are annotated. Following table shows the entities statistics.

| Entity Type | Assembly | Fabricating | Total |
| -- | -- | -- | -- |
| PART | 1,704 | 169 | 1,873 |
| PART_ID |  1,822 | 29 | 1,851 |
| PART_NU | 1,007 | 160 | 1,167 |
| PICTURE | 630 | 12 | 642 |
| PICTURE_VI | 591 | 11 | 602 |
| ATTRIBUTE | 357 | 1,117 | 1,474 |
| ATTRIBUTE_VA | 371 | 1,343 | 1,714 |
| FILE | 1,106 | 893 | 1,999 |
| TOOL | 12 | 319 | 331 |
| OPERATION | 541 | 1,193 | 1,734 |
| ACCESSORY | 79 | 43 | 122 |
| ACCESSORY_ID | 83 | 42 | 125 |
| LOCATION | 104 | 487 | 591 |
| HOLE | 295 | 235 | 530 |
| Total | 8,702  | 6,053  | 14,755 |

## Content

For the fabricating NER data, check the `Data/Fabricating/` folder.

For the assembly NER data, check the `Data/Assembly/` folder.

For total data, check the `Data/Assembly&Fabricating/` folder.

Each folder contains 3 files, `NER`, `NER.data`, `NER.category`,  `NER.summary`, and also cantains 1 folder, CV.

- NER: The entity list.
- NER.data: The annotated sentences.
- NER.category: The entities statistics.
- CV: The data for 10-fold cross validation .
