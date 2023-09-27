# llama2-llm-mac
LLama2 on a Mac

## Create environment

```bash
conda env create -f environment.yaml
```

## Install llama-cpp
```bash
llm install llm-llama-cpp
```

## Install the llama-cpp-python bindings

```bash
pip install llama-cpp-python
```

## Install model

```bash
llm llama-cpp download-model \
  https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGML/resolve/main/llama-2-7b-chat.ggmlv3.q8_0.bin \
  --alias llama2-chat --alias l2c --llama2-chat
```

## Try llama2 out:

```bash
llm -m llama2-chat 'How far is the moon from the earth?'
```
