# Neurosymbolic Hybrid GraphRAG Copilot

A hybrid AI compliance copilot engineered for strict, zero-hallucination regulatory validation in clinical prescription governance.

## Architecture
- **Neural Layer (Probabilistic)**: Entity grounding and intent extraction using a local 4-bit Quantized SLM (`Qwen2.5-3B-Instruct`) and dense vector context retrieval (`ChromaDB` + `bge-small-en-v1.5`).

- **Symbolic Layer (Deterministic)**: Graph relationship traversal via `Neo4j Community` and hard-gated Boolean evaluation via Python rule engine.
- **Delivery**: Dual-panel Streamlit dashboard with real-time Cytoscape/Agraph visual audit trails and downloadable compliance receipts.