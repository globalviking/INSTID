InstantID for Windows 11
===

Instructions:
---

Install Python 3.11 (3.12 or later is not compatible)

Install or upgrade PIP

Clone repository

Create virtual environment

Install dependecies and requirements.

Run app.

```
python.exe -m pip install --upgrade pip
git clone https://github.com/globalviking/INSTID
python -m venv env
pip install torch torchvision torchaudio xformers --index-url https://download.pytorch.org/whl/cu118
pip install -r requirements.txt
python app.py
```

Flags
---

--inbrowser    		Automatically open the url in browser, if --share is used, the public url will be automatically open instead

--server_port    	Choose a specific server port, default=7860 (example --server_port 420    so the local url will be:  http://127.0.0.1:420)

--share				Creates a public URL

--model_path		Name of the sdxl model from huggingface   (the default model example: --model_path stablediffusionapi/juggernaut-xl-v8     diffuser model you can find here: https://huggingface.co/stablediffusionapi/juggernaut-xl-v8

--medvram			Medium vram settings, uses around 13GB, max image resolution of 1024

--lowvram			Low vram settings, uses a bit less than 13GB, max image resolution of 832



---
title: InstantID
emoji: 😻
colorFrom: gray
colorTo: gray
sdk: gradio
sdk_version: 4.15.0
app_file: app.py
pinned: false
license: apache-2.0
---

Check out the configuration reference at https://huggingface.co/docs/hub/spaces-config-reference
