# Hi, I'm Max 👋

IT administrator by day (document management and digitalisation in public administration), AI builder by
night. Trained as an IT systems specialist, studied IT security, taught myself the rest. I run my own AI stack
at home in Balingen, Germany — one workstation, a small k3s cluster and a lot of nights — and I publish what I
find along the way.

> No datacenter. No enterprise budget. Just consumer and workstation hardware and a stubborn refusal to
> accept "unsupported" as the end of the story.

## Released

**[FLE — Fast Local Experts](https://github.com/sirfyyn/FastLocalExperts)** · v1.1.0 · MIT
A llama.cpp fork for running large Mixture-of-Experts models on one 32 GB GPU with the routed experts in host
RAM: a GPU expert cache with a byte budget and warm start, cache hits on the GPU overlapped with misses on the
CPU, MTP speculative decoding with the model's own head, and a leaner prefill. On Qwen3.8-Flash-Next (89 GB)
it decodes at roughly **90 tok/s** in my own paired measurements (RTX PRO 4500 32 GB + Ryzen 9950X3D).
[Technical report](https://sirfyyn.github.io/FastLocalExperts/) ·
[Zenodo](https://doi.org/10.5281/zenodo.23272400) ·
[GGUF models](https://huggingface.co/sirfyyn/Qwen3.8-Flash-Next-FLE-GGUF) ·
[REAP448](https://huggingface.co/sirfyyn/Qwen3.8-Flash-Next-FLE-REAP448-GGUF) ·
[“Making Rhea fast” films](https://www.youtube.com/playlist?list=PLMYhpsBSEhIQ)

**[FLE Studio](https://github.com/sirfyyn/fle-studio)** · v0.3.0 · MIT
A local chat and lab for llama.cpp and the FLE engine: GGUF model loader, live inference data, launch profiles.
No account, no telemetry, macOS, Linux and Windows. [Website](https://sirfyyn.de/fyos/en/studio/)

**[Contexierge](https://github.com/sirfyyn/claude-contexierge)** · Claude Code plugin · MIT
Claude keeps its own session notebook, injected verbatim after every compaction, so what matters survives
long sessions instead of depending on the automatic summary.

## Earlier

| Project | What it is |
|---|---|
| [consumer-llm-patches](https://github.com/sirfyyn/consumer-llm-patches) | 11 patches from fine-tuning Gemma4 26B on a single RTX 4090, with an honest per-patch validation status |
| [three-level-ai-development](https://github.com/sirfyyn/three-level-ai-development) | A method for building with AI: human vision, persistent architect, execution AI |
| [snowmelting-method](https://github.com/sirfyyn/snowmelting-method) | Companion method to the above |

## How I work

- Every claim gets a measurement, and I retract when new evidence says otherwise.
- I build with several AI coding agents in parallel; the decisions stay with me.
- I build for myself first. Sensible issues, PRs and hints are welcome; there is no support promise.

🌐 [sirfyyn.de](https://sirfyyn.de) · 🤗 [huggingface.co/sirfyyn](https://huggingface.co/sirfyyn) · ▶️ [YouTube @sirfyyn](https://www.youtube.com/@sirfyyn)
