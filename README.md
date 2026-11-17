# Multilingual Language Steering (CLaS task, SemEval 2027)

NLP course project, CU Boulder.

We steer an LLM's output language by editing its internal activations at
inference time, with no "respond in X" instruction in the prompt.

Data scripts and evaluation code are adapted from the CLaS organizers:
https://github.com/d-gurgurov/CLaS-SemEval-2027 (MIT, see LICENSE-CLaS).

## Setup
conda create -n clas python=3.11 -y && conda activate clas
pip install datasets huggingface_hub pandas matplotlib ipykernel "numpy==1.26.4" fasttext-wheel
hf auth login
python download_data.py --out data
