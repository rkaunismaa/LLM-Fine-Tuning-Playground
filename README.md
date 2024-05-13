# LLM-Fine-Tuning-Playground

This repo will contain various examples of fine tuning large language models.

*** mamba activate ftllm ***

## Monday, May 13, 2024

Working through [peft_finetuning.ipynb](https://github.com/meta-llama/llama-recipes/blob/main/recipes/finetuning/huggingface_trainer/peft_finetuning.ipynb)

5) mamba install conda-forge::sentencepiece
6) pip install llama-recipes (notice the mis-spelling of recipes)

Trying to understand why running peft_finetuning.ipynb the first time training took 35 minutes, then running it again with profileing enabled from the copied notebook peft_finetuning_2.ipynb it took about a minute and a half, then re-running peft_finetuning_2.ipynb again, but with a different target folder of tmp-profile it again took about a minute and a half ... is this because of something to do with wandb?? I really don't get it ... 

Viewing the first 20 seconds of [LLAMA-3 🦙: EASIET WAY To FINE-TUNE ON YOUR DATA](https://www.youtube.com/watch?v=aQmoog_s8HE) shows me right away there are multiple open-source libraries available to facilitate fine tuning of local large language models. Sooo much energy is being directed at this task and it is rapidly shifting, so keep on this!

The Youtube channel [Prompt Engineering](https://www.youtube.com/@engineerprompt/featured) is excellent! Gonna habituate looking at this channel! 

*** mamba activate unsloth_env ***

Checking out [unsloth](https://github.com/unslothai/unsloth). Create the new conda environment 'unsloth_env' for running the notebook 'Alpaca_+_Llama_3_8b_full_example.ipynb' linked from the page [Finetune Llama 3 - 2x faster + 6x longer context + 68% less VRAM](https://unsloth.ai/blog/llama3)

[Alpaca + Llama-3 8b full example.ipynb](https://colab.research.google.com/drive/135ced7oHytdxu3N2DNe1Z0kqjyYIkDXp?usp=sharing)

Damn! My preliminary dive into unsloth is revealing some fantastic features of this package!

I was able to run 'Alpaca_+_Llama_3_8b_full_example.ipynb' in unsloth_dev with no problems!

Now will create a second conda environment almost identical to unsloth_env bit with a slightly different setup, supposedly catered to a 4090, and will name it unsloth_env2 ... I know ... really creative, right!?

* [LLAMA-3 🦙: EASIET WAY To FINE-TUNE ON YOUR DATA 🙌](https://www.youtube.com/watch?v=aQmoog_s8HE)
* https://colab.research.google.com/drive/1mPw6P52cERr93w3CMBiJjocdTnyPiKTX#scrollTo=2eSvM9zX_2d3

## Sunday, May 12, 2024

Noteable links:

* [Using and Finetuning Pretrained Transformers](https://magazine.sebastianraschka.com/p/using-and-finetuning-pretrained-transformers)
* [Finetuning Large Language Models](https://magazine.sebastianraschka.com/p/finetuning-large-language-models)
* [Fine-tuning 20B LLMs with RLHF on a 24GB consumer GPU](https://huggingface.co/blog/trl-peft)
* [A Gentle Introduction to 8-bit Matrix Multiplication for transformers at scale using Hugging Face Transformers, Accelerate and bitsandbytes](https://huggingface.co/blog/hf-bitsandbytes-integration)

## Saturday, May 11, 2024

Starting to run through the notebook 'Causal_models_like_Gemma_2B_finetuning_on_SamSum.ipynb', and looks like I have more stuff to install ...

 1) mamba install conda-forge::huggingface_hub
 2) mamba install conda-forge::ipywidgets
 3) pip install evaluate
 4) pip install rouge-score


