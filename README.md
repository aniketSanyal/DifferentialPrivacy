# Differential Privacy
The above repository encompasses code for the following 5 techniques used for tuning Large Language Models -
1. soft prompt
2. prefix tuning
3. full fine tuning
4. Low Rank Adaption (LORA)
5. last layer fine tuning

The chose model is tiny-bert ("prajjwal1/bert-tiny"), trained on the datasets "sst2", "qnli", "qqp" and "mnli"

Please run the following command before running on colab to install dependencies

```
pip install peft opacus transformers datasets loralib
```

Primarily, I tuned the optimiser with learning rates of 1e-3 and 5e-4. The batch sizes were also tuned around ranging from 8-256
