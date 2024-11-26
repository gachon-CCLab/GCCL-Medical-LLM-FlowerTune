# GCCL-Medical-LLM-FlowerTune

### Evaluation for Medical challenge (Result of 10th checkpoint out of 10 total rounds)

|        | PubMedQA | MedMCQA | MedQA |  Avg  |
| :-----: | :------: | :-----: | :---: | :---: |
| Acc (%) |   70.6   |  57.68  | 61.50 | 63.26 |

#### Changes from baseline

<pyproject.toml>

`model.name = "ContactDoctor/Bio-Medical-Llama-3-8B"`

`num-server-rounds = 10`

#### Evaluation Command

```
python eval.py \
--base-model-name-path=ContactDoctor/Bio-Medical-Llama-3-8B \
--peft-path= \ # PEFT PATH - Checkpoint 10
--run-name= \ # RUN NAME
--batch-size=16 \
--quantization=4 \
--datasets=pubmedqa,medmcqa,medqa
```


### Evaluation for Medical challenge (Result of 100th checkpoint out of 100 total rounds)

|        | PubMedQA | MedMCQA | MedQA | Avg |
| :-----: | :------: | :-----: | :---: | :--: |
| Acc (%) |   71.6   |  52.47  | 52.08 | 58.8 |

#### Changes from baseline

<pyproject.toml>

`model.name = "ContactDoctor/Bio-Medical-Llama-3-8B"`

`num-server-rounds = 100`

#### Evaluation Command

```
python eval.py \
--base-model-name-path=ContactDoctor/Bio-Medical-Llama-3-8B \
--peft-path= \ # PEFT PATH - Checkpoint 100
--run-name= \ # RUN NAME
--batch-size=16 \
--quantization=4 \
--datasets=pubmedqa,medmcqa,medqa
```
