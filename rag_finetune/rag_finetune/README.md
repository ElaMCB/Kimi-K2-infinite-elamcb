# 128 k-RAG pipeline for Kimi K2
## Quick start
1. Put LoRA `*.safetensors` in `checkpoints/`
2. Put FAISS index + metadata DB in `data/`
3. Run `scripts/03_finetune_rag.sh`

## Scripts
- `01_build_index.sh`   – chunk + embed corpus → FAISS
- `02_make_rag_data.py` – build 128 k retrieval mixtures
- `03_finetune_rag.sh`  – launch DeepSpeed training

## Weights
`checkpoints/k2-rag-lora-8bit-128k/`
(upload your files here)

## Data
`data/faiss_k2.ivf16384_pq64.faiss`  
`data/chunks.sqlite3`
