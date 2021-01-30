# NER-for-Manufacturing-WI

This repository contains a named entity recognition (NER) corpus for Chinese manufacturing work instruction (WI).

## Contributer
- Peiyan Wang

## Overview
This corpus contains 709 fabricating WI sentences,  774 assembly WI sentences,  and total 427,656 characters.  Fourteen types of entities are annotated. Following table shows the entities statistics.

| Entity Type | Assembly | Fabricating | Total | Description |
| -- | -- | -- | -- | -- |
| PART | 1,704 | 169 | 1,873 | The name of the part to be assembled or fabricated (e.g., 面板/Panel, 螺钉/Screw). |
| PART_ID |  1,822 | 29 | 1,851 | The identification number of the part to be assembled or fabricated (e.g., 201C407-777-7HI, NAS20426). |
| PART_NU | 1,007 | 160 | 1,167 | The quantity of part required for assembly or fabricated (e.g., 4个/Four, 6组/6 groups). |
| PICTURE_ID | 630 | 12 | 642 | The identification number or name of engineering documents to be followed during manufacturing (e.g., BR270347-799HH). |
| PICTURE_VI | 591 | 11 | 602 | The name of manufacturing operation (e.g., 钻/Drill, 铣/Milling). |
| ATTRIBUTE | 357 | 1,117 | 1,474 | The identification number of the drawing for manufacturing (e.g.,905C1877-777-7HI). |
| ATTRIBUTE_VA | 371 | 1,343 | 1,714 | The drawing view requiring special attention in manufacturing operations (e.g., B-B视图/B-B views). |
| FILE | 1,106 | 893 | 1,999 | The name of tool used in manufacturing operation (e.g., 钻头/Drilling bit). |
| TOOL | 12 | 319 | 331 | The part manufacturing area (e.g., 顶端/Top, 钩面/Hook surface). |
| OPERATION | 541 | 1,193 | 1,734 | The hole in part (e.g., 排液孔/Drain hole). |
| ACCESSORY | 79 | 43 | 122 | The name of process accessory used in manufacturing (e.g., 底漆/Primer). |
| ACCESSORY_ID | 83 | 42 | 125 | The identification number of process accessory used in manufacturing (e.g., BO28453HT). |
| PART_AR | 104 | 487 | 591 | The attribute of part or manufacturing operation (e.g., 粗糙度/Roughness, 孔径/Diameter). |
| HOLE | 295 | 235 | 530 | The attribute value of part or manufacturing operation attribute (e.g., 0.202英寸/0.202 inch).
| Total | 8,702  | 6,053  | 14,755 |   |

## Content

For the fabricating NER data, check the `Data/Fabricating/` folder.

For the assembly NER data, check the `Data/Assembly/` folder.

For total data, check the `Data/Assembly&Fabricating/` folder.

Each folder contains 3 files, `NER`, `NER.data`, `NER.category`,  `NER.summary`, and also cantains 1 folder which is `CV`.

- `NER`: The entity list.
- `NER.data`: The annotated sentences.
- `NER.category`: The entities statistics.
- `CV`: The data for 10-fold cross validation .
