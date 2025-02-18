# Phi-2 DialogSum Fine-tuned

This repository contains a Jupyter Notebook for fine-tuning the Phi-2 model on the DialogSum dataset.

## Project Overview
The notebook is designed to train a large language model using the [DialogSum dataset](https://huggingface.co/datasets/neil-code/dialogsum-test). It leverages Hugging Face Transformers and other machine learning libraries to enhance the model's ability to summarize dialogues effectively.

## Requirements
- Python 3.x
- Hugging Face Transformers
- PyTorch
- ROUGE Score for evaluation
- Other standard ML libraries

## Usage
To run the notebook:
```sh
pip install -r requirements.txt
jupyter notebook phi-2-dialogsum-finetuned.ipynb
```

## References
- [DialogSum Dataset](https://huggingface.co/datasets/neil-code/dialogsum-test)
- [Fine-tuning Guide](https://ai.stackexchange.com/questions/41485)
- [Model in huggingface](https://huggingface.co/mursuturpa/phi-2-dialogsum-finetuned)

# Errors fixed
- Fixed error "AttributeError: module 'rouge_score' has no attribute '__version__'.""
- Library was not installed !pip install pynvml
- Train the fine-tuned model with the following configuration, which had to be edited
    a. max_steps = 500
    b. logging_steps = 50
    c. eval_steps = 50
  - Corrected path to Peft model

## License
-
