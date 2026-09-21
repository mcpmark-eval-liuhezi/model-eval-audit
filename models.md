# Hugging Face Hub Model Snapshot

Source of truth: Hugging Face Hub, model **`google-bert/bert-base-uncased`**.
Fetched from the Hub API on **2026-09-21T07:58Z** (UTC), with a browser cross-check of the model page in the same session.

## Stats (exactly as returned by the Hub API right now)

| Field | Value |
|---|---|
| Pipeline task tag | `fill-mask` |
| License | `apache-2.0` |
| Downloads | 3,238,100,000 (API renders it as "3238.1M") |
| Likes | 3,366 |
| Last repo update | 19 Feb, 2024 |
| Library / model class | `transformers` / `AutoModelForMaskedLM` |
| Parameters | 110.1M |
| Language | `en` |

Metric note: the Hub API figure above is the model's reported download total. The model *page* widget showed **"Downloads last month: 46,140,403"** at the same moment — that is a 30-day window, not the same metric.

## Repository files (root, from `ls` on the Hub repo)

| File | Size | Notes |
|---|---|---|
| `.gitattributes` | 491 B | |
| `LICENSE` | 11.4 KB | |
| `README.md` | 10.5 KB | |
| **`config.json`** | 570 B | required artifact — present |
| `flax_model.msgpack` | 438.1 MB | LFS |
| `model.onnx` | 532.1 MB | LFS |
| `model.safetensors` | 440.4 MB | LFS |
| `pytorch_model.bin` | 440.5 MB | LFS |
| `rust_model.ot` | 534.2 MB | LFS |
| `tf_model.h5` | 536.1 MB | LFS |
| `tokenizer.json` | 466.1 KB | |
| `tokenizer_config.json` | 48 B | |
| **`vocab.txt`** | 231.5 KB | vocab file — present |

There is also one directory, `coreml/` (Core ML package under `coreml/fill-mask/float32_model.mlpackage/`).

### Artifact presence check (pre-commit gate)

- `config.json` — **present** at repo root (570 B)
- vocab file — **present**: `vocab.txt` at repo root (231.5 KB), alongside `tokenizer.json` (466.1 KB) and `tokenizer_config.json` (48 B)

## Browser cross-check (model page vs. API)

Model page opened at https://huggingface.co/google-bert/bert-base-uncased during the same session.

| Item | API says | Page shows | Verdict |
|---|---|---|---|
| Task tag | `fill-mask` | `Fill-Mask` (tag chip in header) | **Match** — display-case difference only, no mismatch |
| License | `apache-2.0` | `apache-2.0` | **Match** — no mismatch |
| Likes | 3,366 | `3.37k` (header) | Consistent (page shows rounded value) |
| Downloads | 3,238,100,000 total | 46,140,403 "Downloads last month" | Different metrics (total vs 30-day), not a contradiction |

No mismatch found between the Hub website and the Hub API for the task tag or the license.

## Related artifacts

- Briefing deck: `model_eval_brief.pptx` — slide 1 "Model Evaluation Briefing", slide 2 "google-bert/bert-base-uncased" with a downloads-vs-likes bar chart (3,238,100,000 vs 3,366).
