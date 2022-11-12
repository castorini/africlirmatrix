# AfriCLIRMatrix: Enabling Cross-Lingual Information Retrieval for African Languages

AfriCLIRMatrix is a novel dataset for cross-lingual information retrieval in 11 geographically diverse African languages.

## Results
Baseline BM25, mDPR (fine-tuned on ms marco) and sparse-dense hybrid results on Africlirmatrix

### nDCG@10
|                |   Afr  |   Amh  |   Ary  |   Arz  |   Hau  |   Ibo  |  Nso  |  Sna  |   Som  |   Swa  |   Tir  |   Twi  |   Wol  |   Yor  |   Zul  |  avg  |
|----------------|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|
| BM25 (default) | 0.434 | 0.159 | 0.167 | 0.268 | 0.508 | 0.518 | 0.445 | 0.262 | 0.305 | 0.418 | 0.080 | 0.513 | 0.134 | 0.484 | 0.247 | 0.329 |
| mDPR (MS Marco) | 0.309 | 0.215 | 0.355 | 0.118 | 0.269 | 0.338 | 0.282 | 0.351 | 0.218 | 0.335 | 0.265 | 0.333 | 0.232 | 0.377 | 0.178 | 0.281 |
| Hybrid |  0.464 | 0.228 | 0.350 | 0.257 | 0.508 | 0.580 | 0.526 | 0.394 | 0.344 | 0.477 | 0.239 | 0.547 | 0.233 | 0.532 | 0.273 | 0.397 |

### Recall@100
|                |    Afr  |   Amh  |   Ary  |   Arz  |   Hau  |   Ibo  |  Nso  |  Sna  |   Som  |   Swa  |   Tir  |   Twi |   Wo  |   Yo  |   Zu  |  avg  |
|----------------|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|
| BM25 (default) | 0.584 | 0.174 | 0.224 | 0.309 | 0.650 | 0.685 | 0.629 | 0.346 | 0.403 | 0.556 | 0.080 | 0.560 | 0.166 | 0.627 | 0.289 | 0.418 |
| mDPR (MS Marco) |  0.591 | 0.382 | 0.694 | 0.248 | 0.542 | 0.668 | 0.670 | 0.642 | 0.445 | 0.595 | 0.580 | 0.664 | 0.548 | 0.655 | 0.361 | 0.552 | 
| Hybrid |  0.727 | 0.388 | 0.698 | 0.416 | 0.722 | 0.804 | 0.766 | 0.684 | 0.535 | 0.690 | 0.600 | 0.732 |0.556 | 0.750 | 0.448 | 0.634 |

## Citation
If you find our paper useful or use the dataset in your work, please cite our paper and the CLIRMatrix paper:


```bash
@inproceedings{sun-duh-2020-clirmatrix,
    title = "{CLIRM}atrix: A massively large collection of bilingual and multilingual datasets for Cross-Lingual Information Retrieval",
    author = "Sun, Shuo  and
      Duh, Kevin",
    booktitle = "Proceedings of the 2020 Conference on Empirical Methods in Natural Language Processing (EMNLP)",
    month = nov,
    year = "2020",
    address = "Online",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2020.emnlp-main.340",
    doi = "10.18653/v1/2020.emnlp-main.340",
    pages = "4160--4170",
    abstract = "We present CLIRMatrix, a massively large collection of bilingual and multilingual datasets for Cross-Lingual Information Retrieval extracted automatically from Wikipedia. CLIRMatrix comprises (1) BI-139, a bilingual dataset of queries in one language matched with relevant documents in another language for 139x138=19,182 language pairs, and (2) MULTI-8, a multilingual dataset of queries and documents jointly aligned in 8 different languages. In total, we mined 49 million unique queries and 34 billion (query, document, label) triplets, making it the largest and most comprehensive CLIR dataset to date. This collection is intended to support research in end-to-end neural information retrieval and is publicly available at [url]. We provide baseline neural model results on BI-139, and evaluate MULTI-8 in both single-language retrieval and mix-language retrieval settings.",
}
```

## Contact us
If you have any question or suggestions regarding the dataset, code or publication, 
please contact Ogundepo Odunayo (oogundep[at]uwaterloo.ca)

