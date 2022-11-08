# Assignment 3: Improving Low-Resource NMT

In this assignment we use fr-en data from the Tatoeba
corpus and investigate methods for improving low-resource NMT.

Your task is to experiment with techniques for improving
low-resource NMT systems.

## Baseline

The data used to train the baseline model was prepared using
the script `preprocess_data.sh`.
This may be useful if you choose to apply subword
segmentation or a data augmentation method.


## Lexical Model
This folder contains the checkpoints(best and last) of lexical model. The file translations.p.txt is the translated English of test set by using the lexical modle. Added some code in the decoder part of file seq2seq/models/lstm.py.

BLEU score: 
{ 
 "name": "BLEU",
 "score": 23.1,
 "signature": "nrefs:1|case:mixed|eff:no|tok:13a|smooth:exp|version:2.2.1",
 "verbose_score": "53.5/29.4/17.3/10.6 (BP = 1.000 ratio = 1.152 hyp_len = 4485 ref_len = 3892)",
 "nrefs": "1",
 "case": "mixed",
 "eff": "no",
 "tok": "13a",
 "smooth": "exp",
 "version": "2.2.1"
}
