# FuzzyLLM: Fuzzy Logic Controller for Large Language Models

Fuzzy Logic Controller for LLM text generation (FuzzyLLM) with GPT-2 implementation and spam classifier fine-tuning

Monograph: "Architecture of Large Language Models with Fuzzy Logic Generation Control"  
Bobyr M.V., 2026

## Repository Structure

| File | Chapter | Content |
|------|---------|---------|
| LLM_Chapter1.ipynb | Chapter 1 | Text preprocessing, BPE tokenization, stride* regulator |
| LLM_Chapter2.ipynb | Chapter 2 | Self-attention mechanism, τ* regulator |
| LLM_Chapter3.ipynb | Chapter 3 | GPT-2 architecture, β* regulator |
| LLM_Chapter4.ipynb | Chapter 4 | Training, decoding strategies, OpenAI weights |
| LLM_Chapter5_FuzzyLLM.ipynb | Chapter 5 ★ | FuzzyLLM controller (original contribution) |
| LLM_Chapter6.ipynb | Chapter 6 | Fine-tuning for spam classification |

★ Chapter 5 is the original scientific contribution of this work.

## Key Experimental Results

- Entropy reduction during generation: 3.1× (no weight changes)
- Average β* vs standard: −34.7%
- Average τ* vs standard √2: −39.7%
- Spam classifier accuracy (test set): 95.67%
- Training time on CPU: ~10 minutes

## Installation
```bash
pip install torch tiktoken numpy matplotlib pandas
pip install tensorflow>=2.15.0 tqdm>=4.66
```

## How to Run

Open any `.ipynb` file in Jupyter Notebook and run cells sequentially.  
GPU is not required; all experiments reproduce on CPU.

## Citation
```
Bobyr M.V. Large Language Model Architecture and Fuzzy Logic Control 
of Text Generation. 2026.
GitHub: https://github.com/MaxBobyr1978/fuzzy-llm-controller
```
