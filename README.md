# DIY LLM Infra

See [PURPOSE.md](PURPOSE.md) and [ROADMAP.md](ROADMAP.md) for full project details.

---

## Quick Reference

### Inference Engines

| Engine | Type | Notes |
|---|---|---|
| llama.cpp | Native C/C++ | GGUF format, CUDA support, full control |
| vLLM | Python server | High-throughput serving, PagedAttention, tensor parallelism |
| Ollama | CLI / API wrapper | Easiest setup, OpenAI-compatible API |
| SGLang | Python server | Structured generation, fast serving |
| Unsloth | Desktop app / Python | Local UI for inference and fine-tuning, GGUF support |

## References

External links and additional references will be added as documentation matures.

## Notes

- Partial GPU offload strategy: larger models spill to system RAM when they exceed VRAM
- All API access is behind WireGuard, no authentication required on the local side
