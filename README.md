# 😜LoRACSE: Contrastive Learning of Sentence Embedding using LoRA
##  Final project of EECS 487: Introduction to Natural Language Processing (Umich)
### autor: Yilin Jia, Sikai Li, Yuqi Mai
### date: 18/4/2013

## Instructions

- Open the LoraCSE.ipynb notebook to access the code of all the experiments.
- Follow the instructions provided in the notebook to run the experiments with your GPU and view the results.
- The detail of experiments is shown in LoRACSE.pdf.

## Performance

|              Model              | Avg. STS |
|:-------------------------------|:--------:|
| sup-loracse-bert-base (batch size 512) |  81.55  |
| sup-loracse-roberta-base (batch size 512) |   82.49  |
| sup-loracse-roberta-large (batch size 375) |   84.69  |

## Requirements

To run the experiment, which involves processing large amounts of data with a batch size of 512, your GPU must have at least 40GB of RAM.
Here are the compatible GPUs:

- V100
- A6000
- A40
- RTX3090 (four required)

In this experiment, we use four A40.


## Acknowledgements

We would like to acknowledge the following projects for their contributions to our work:

- [SimCSE](https://github.com/princeton-nlp/SimCSE): Our code has learned a lot from the implementation and ideas presented in this repository.
- [PEFT](https://github.com/huggingface/peft): We have used some of the functionality provided by this library to improve the performance of our code.

We are grateful to the contributors of these projects for sharing their knowledge and expertise with the community.

## Future work
- Learn and use adalora to tune.
- Accelerate the training and evaluation.
- Try to tune debertv3.
- Upload the model to Huggingface.
