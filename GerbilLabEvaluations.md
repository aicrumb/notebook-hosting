
<img src="https://media.discordapp.net/attachments/1074346695191711875/1090859826793431139/image.png?width=1031&height=152" width=100%\>

Who needs em, we all have em, they're just like us. Unusable models, compute optimally 🔥. We hope that by open-sourcing our compute-optimal trained models, that others can replicate our results and also make no use out of our unusable models. These models are not useful in the slightest, and don't benefit research. Every time you use one of these models, you can be sure that you will not get a useful result, and every time we kiss I swear I can fly. Can't you feel my heart beat fast, I want this to last, need you by my side. We introduce a cascade(a) (sorry) of classes and models:

- A-Class Models: 20 x Million Params tokens in training set. (Chinchilla-Optimal)
- B-Class Models: 42 x Million Params tokens in training set.
- C-Class Models: 76 x Million Params tokens in training set.
- D-Class Models: 142 x Million Params tokens in training set.

The B, C, and D classes are derived from the tokens per model ratio from LLaMA, as LLaMA 65B is nearly Chinchilla-optimal with a ratio of 21 x Million Params tokens in training. Descending down the model sizes per training set for each model gives us these classes. Any "star" class model is approximately the class but not exactly, and finetuned from a previous checkpoint for time-saving purposes.

| Model Name | Parameters | Class | Ratio | Tokens | Batch Size (Tokens) | Training Loss ↓ | hellaswag acc ↑ | lambada ppl ↓ | lambada acc ↑ | winogrande acc ↑
| --- | --- | --- | --- | --- |  --- |  --- |   --- |   --- |   --- |   --- | 
| **[GerbilLab/Gerbil-A-6.7m](https://hf.co/GerbilLab/Gerbil-A-6.7m)** | 6.7m | A-Class | 20 | 134M | 131k | 6.0741 | 26.04 | 614655.4052 | 0 | 51.7 |
| [GerbilLab/Gerbil-B-6.7m](https://hf.co/GerbilLab/Gerbil-B-6.7m) | 6.7m | B-Class | 42 | 281M | 131k | 5.5132 | 25.74 | 370243.6771 | 0 | 52.64 |
| [GerbilLab/Gerbil-C-6.7m](https://hf.co/GerbilLab/Gerbil-C-6.7m) | 6.7m | C-Class | 76 | 509M | 131k | 5.1098 | 25.54 | 199753.1491 | 0 | 52.72 |
| [GerbilLab/Gerbil-D-6.7m](https://hf.co/GerbilLab/Gerbil-D-6.7m) | 6.7m | D-Class | 142 | 852M | 131k | 4.8186 | 25.32 | 127810.4082 | 0 | 52.88 |
| **[GerbilLab/Gerbil-A-15m](https://hf.co/GerbilLab/Gerbil-A-15m)** | 15m | A-Class | 20 | 280M | 131k | 4.9999 | 25.56 | 190773.1317 | 0 | 52.17 |
| **[GerbilLab/Gerbil-A-32m](https://hf.co/GerbilLab/Gerbil-A-32m)** | 32m | A-Class | 20 | 640M | 262K | 4.0487 | 25.9 | 19358.5197 | 0.83 | 51.14 |
| --- | --- | --- | --- | --- |  --- |  --- | 
| **[GerbilLab/GerbilBlender-A-6.7m](https://hf.co/GerbilLab/GerbilBlender-A-6.7m)** | 6.7m | A-Class | 20 | 134M | 131k | 6.0908 | 26 | 627506.0021 | 0 | 50.12 |
| **[GerbilLab/GerbilBlender-D-6.7m](https://hf.co/GerbilLab/GerbilBlender-D-6.7m)** | 6.7m | D-Class | 142 | 852M | 131k |4.838100 | 25.55 | 151087.4082 | 0.02 | 51.3 |
| **[GerbilLab/GerbilBlender-E-star-6.7m](https://hf.co/GerbilLab/GerbilBlender-E-star-6.7m)** | 6.7m | E*-Class | 284 | 1704M | 131k-262k | 4.7547 | 25.47 | 122411.0728 | 0.06 | 50.59 |
| **[GerbilLab/GerbilBlender-A-15m](https://hf.co/GerbilLab/GerbilBlender-A-15m)** | 15m | A-Class | 20 | 280M | 131k | 4.9642 | 25.8 | 203830.1811 | 0 | 49.96 |
| **[GerbilLab/GerbilBlender-A-32m](https://hf.co/GerbilLab/GerbilBlender-A-32m)** | 32m | A-Class | 20 | 640M | 262K | 4.127 | 25.81 | 16491.0141 | 2.66 | 51.93 |
| **[GerbilLab/GerbilBlender-A-77m](https://hf.co/GerbilLab/GerbilBlender-A-77m)** | 77m | A-Class | 20 | 1520M | 262K | 3.3334 | 26.06 | 1908.0661 | 18.2 | 52.09 |
| **[GerbilLab/GerbilBlender-B-star-77m](https://hf.co/GerbilLab/GerbilBlender-B-star-77m)** | 77m | B*-Class | 40 | 3040M | 262K-524K | 3.1879 | 26.33 | 1766.5002 | 18.24 | 53.43 |
| **[GerbilLab/GerbilBlender-C-star-77m](https://hf.co/GerbilLab/GerbilBlender-C-star-77m)** | 77m | C*-Class | 60 | 4560M | 262K-524K | coming soon |
| **[GerbilLab/GerbilBlender-A-104m](https://hf.co/GerbilLab/GerbilBlender-A-104m)** | 104m | A-Class | 20 | 2060M | 1M (too big, would outperform a-77 if was using 524k)| 3.592 | 26.41 | 2972.4260 | 17.31 | 49.6 |
| --- | --- | --- | --- | --- |  --- |  --- | 
| GerbilLab/GerbilCode-6.7m | 6.7m | . | ~300 | 2852M | 131k | 3.98 | 25.4 | 124001.9108 | 0.08 | 52.72 |
<!---
| [GerbilLab/T5Blender-A-24m](https://hf.co/GerbilLab/T5Blender-A-24m) | 24m | A-class | 20 | 460M | 131K | 5.5642 | 25.85 | 57122770.9237 | 0 | 52.25 |
| [GerbilLab/T5Blender-B-star-24m](https://hf.co/GerbilLab/T5Blender-B-star-24m) | 24m | B*-Class | 40 | 920M | 131K-262K | 5.419 | 
| [GerbilLab/T5Blender-C-star-24m](https://hf.co/GerbilLab/T5Blender-C-star-24m) | 24m | C*-Class | 60 | 1380M | 131K-262K | coming soon | 

--->
Scores to beat:

| Model Name | Parameters | Tokens | hellaswag | lambada ppl | lambada acc | winogrande acc |
| --- | --- | --- | --- | --- | --- | --- |
| EleutherAI/pythia-70m-deduped | 70m | 300B(?) |27.36 | 90.5683 | 25.25 | 52.25 |

Nearly every base model that isn't finetuned for a specific task was trained on the deduplicated Pile dataset, and is a Decoder-only model. "Blender" models, inspired by UL2 pretraining, are trained equally in fill-in-the-middle, causal modelling, and masked language modelling tasks. Special tokens for these models include:

```
'<fitm_start>', '<multiple_tok_mask>', '<fitm_result>', '<causal>', '<mlm_start>', '<single_tok_mask>', '<mlm_end>'

# Example fill in the middle
'<fitm_start> this is an <multiple_tok_mask> for fill-in-the-middle <fitm_result> example text <|endoftext|>'

# Example causal language modelling
'<causal> this is an example text for causal language modelling <|endoftext|>'

# Example masked language modelling
'<mlm_start> this is an <single_tok_mask> text for masked language modelling <mlm_end> example <|endoftext|>'

```

Some applications where I can imagine these being useful are: warm-starting very small encoder-decoder models, fitting a new scaling law that takes into account smaller models, or having a "fuzzy wrapper" around an API. They also could be usable on their own (for classification or other) when finetuned on more specific datasets. I don't expect the 3.3m models to be useful for any task whatsoever. Every model was trained on a singular GPU, either a RTX2060, RTX3060, or a T4. 

I'd , uh , appreciate help in evaluating all these models probably with lm harness!!

Other "small-scale" models that are not Gerbil/Blender but still beneficial to low-resource neural computing that I create will be uploaded here as well. 
