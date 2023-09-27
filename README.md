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
llm install https://static.simonwillison.net/static/2023/llama_cpp_python-0.1.77-cp311-cp311-macosx_13_0_arm64.whl
```

## Install model

```bash
llm llama-cpp download-model \
  https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGML/resolve/main/llama-2-7b-chat.ggmlv3.q8_0.bin \
  --alias llama2-chat --alias l2c --llama2-chat
```

## Try llama2 out:

```bash
llm -m l2c 'How far is the moon from the earth?'
```
