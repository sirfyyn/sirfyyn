# Hi, I'm Max 👋

IT administrator by day (document management and digitalisation in public administration), AI builder by
night. Trained as an IT systems specialist, studied IT security, taught myself the rest. I run my own AI stack
at home in Balingen, Germany — one workstation, a small k3s cluster and a lot of nights — and I publish what I
find along the way.

> No datacenter. No enterprise budget. Just consumer and workstation hardware and a stubborn refusal to
> accept "unsupported" as the end of the story.

## What I'm working on

**FLE — Fast Local Experts** · `fle.cpp` *(release in preparation)*
A llama.cpp-based engine for running large Mixture-of-Experts models on a single 32 GB GPU with the
experts in system RAM: an expert cache with overlapped transfers, a self-trained MTP head for
speculative decoding, and a leaner prefill path. On Qwen3.8-Flash-Next it decodes at roughly
**90 tok/s** in my own paired measurements (RTX PRO 4500 32 GB + Ryzen 9950X3D).
Model, measurements and a write-up will follow on [Hugging Face](https://huggingface.co/sirfyyn).

**FYOS** · *private*
My personal AI operating system: local models, agents, home automation and the tooling that ties them
together, running on my own cluster.

## Published

| Project | What it is |
|---|---|
| [consumer-llm-patches](https://github.com/sirfyyn/consumer-llm-patches) | 11 patches from fine-tuning Gemma4 26B on a single RTX 4090, with an honest per-patch validation status |
| [three-level-ai-development](https://github.com/sirfyyn/three-level-ai-development) | A method for building with AI: human vision, persistent architect, execution AI |
| [snowmelting-method](https://github.com/sirfyyn/snowmelting-method) | Companion method to the above |

## How I work

- Every claim gets a measurement, and I retract when new evidence says otherwise.
- I build for myself first. Sensible issues, PRs and hints are welcome; there is no support promise.

🌐 [sirfyyn.de](https://sirfyyn.de) · 🤗 [huggingface.co/sirfyyn](https://huggingface.co/sirfyyn)
