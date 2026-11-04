# Hi, I'm Max 👋

IT administrator by day (document management and digitalisation in public administration), AI builder by
night. Trained as an IT systems specialist, studied IT security, taught myself the rest. I run my own AI stack
at home in Balingen, Germany — one workstation, a small k3s cluster and a lot of nights — and I publish what I
find along the way.

> No datacenter. No enterprise budget. Just consumer and workstation hardware and a stubborn refusal to
> accept "unsupported" as the end of the story.

## Released

**[FLE Link](https://github.com/sirfyyn/flelink)** · v0.1.4 · MIT · [flelink.run](https://flelink.run)
Run local AI models with one file and one command: it checks the machine, installs the right engine, finds or
downloads the model (every file checked by its SHA-256) and serves an OpenAI- and Anthropic-compatible API, with a
Studio for chat, live numbers and recipes. 66 s from nothing to the first answer on Linux, 68 s on an 8 GB MacBook.
DeepSeek-V4.1-Flash (232 GiB) runs at **31.6 tok/s** through FLE Link on one 32 GB GPU (best performance measured on Linux).

**[FLE — Fast Local Experts](https://github.com/sirfyyn/FastLocalExperts)** · v1.2.4 · MIT
A llama.cpp fork for large Mixture-of-Experts models on one 32 GB GPU with the routed experts in host RAM: a GPU
expert cache with a byte budget and warm start, a RAM expert store, prefill windows, MTP and DSpark speculative
decoding. Qwen3.8-Flash-Next (89 GB) at roughly **90 tok/s**; DeepSeek-V4.1-Flash exact at **33.3 tok/s**, with the
DSpark draft model 41.9 (RTX PRO 4500 32 GB + Ryzen 9950X3D, 120 GB RAM, my own measurements). Best performance measured on Linux.
[Technical report](https://sirfyyn.github.io/FastLocalExperts/) ·
[Zenodo](https://doi.org/10.5281/zenodo.23272400) ·
[“Making Rhea fast” films](https://www.youtube.com/playlist?list=PLMYhpsBSEhIQ)

**[FYOS — For Your Own Sake](https://github.com/sirfyyn/fyos-os)** · 0.3 · Apache-2.0
A personal operating system in the browser: desktop shell, MCP hub and installer, with
[an agent foundation](https://github.com/sirfyyn/fyos-agent) and plugins for mail, calendars, the home, finances
and operations. Runs entirely on your side.

**[FLE Durable](https://github.com/sirfyyn/fle-durable)** · Apache-2.0
An always-on local agent that works from events: agenda, webhooks, one durable queue; survives restarts without
losing or repeating anything. Runs with FLE Link or any OpenAI-compatible model.

**[Contexierge](https://github.com/sirfyyn/claude-contexierge)** · Claude Code plugin · MIT
Claude keeps its own session notebook, injected verbatim after every compaction, so what matters survives long
sessions instead of depending on the automatic summary.

## Models on Hugging Face

| Model | What it is |
|---|---|
| [Qwen3.8-Flash-Next-FLE-GGUF](https://huggingface.co/sirfyyn/Qwen3.8-Flash-Next-FLE-GGUF) | FLE quants of a 125B MoE, smaller than Unsloth's at the same KL divergence |
| [Qwen3.8-Flash-Next-FLE-REAP448-GGUF](https://huggingface.co/sirfyyn/Qwen3.8-Flash-Next-FLE-REAP448-GGUF) | the same with 64 of 512 experts per layer pruned by REAP |
| [DeepSeek-V4.1-Flash-1017-DSpark-FLE-GGUF](https://huggingface.co/sirfyyn/DeepSeek-V4.1-Flash-1017-DSpark-FLE-GGUF) | the DSpark draft model for DeepSeek-V4.1-Flash on FLE (lossless at temperature 0) |
| [Katy-27B-GGUF](https://huggingface.co/sirfyyn/Katy-27B-GGUF) | GGUF quants of Swift-1.5-Qwen3.8-27b |

## Earlier

| Project | What it is |
|---|---|
| [FLE Studio](https://github.com/sirfyyn/fle-studio) | the Python predecessor of FLE Link's Studio |
| [consumer-llm-patches](https://github.com/sirfyyn/consumer-llm-patches) | 11 patches from fine-tuning Gemma4 26B on a single RTX 4090, with an honest per-patch validation status |
| [three-level-ai-development](https://github.com/sirfyyn/three-level-ai-development) | A method for building with AI: human vision, persistent architect, execution AI |
| [snowmelting-method](https://github.com/sirfyyn/snowmelting-method) | Companion method to the above |

## How I work

- Every claim gets a measurement, and I retract when new evidence says otherwise.
- I build with several AI coding agents in parallel; the decisions stay with me.
- I build for myself first. Sensible issues, PRs and hints are welcome; there is no support promise.

🌐 [sirfyyn.de](https://sirfyyn.de) · 🔗 [flelink.run](https://flelink.run) · 🤗 [huggingface.co/sirfyyn](https://huggingface.co/sirfyyn) · ▶️ [YouTube @sirfyyn](https://www.youtube.com/@sirfyyn)
