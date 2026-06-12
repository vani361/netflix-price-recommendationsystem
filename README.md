# Netflix Recommendation System

Two-stage collaborative filtering pipeline:
- **Stage 1**: WALS (Weighted Alternating Least Squares) — retrieval & rating prediction
- **Stage 2**: BPR (Bayesian Personalised Ranking) — reranking

## Results
| Model | RMSE | MAP@10 |
|-------|------|--------|
| WALS | ~0.97 | 0.0184 |
| WALS + BPR (N=2000) | — | **0.0482** |

## Files
- `train_wals.py` — WALS training script
- `bpr_model.py` — BPR reranker
- `explain_recommendations_v2.py` — Explainable recommendations
- `generate_final_predictions.py` — Inference pipeline
- `*.ipynb` — Training notebooks

## Dataset
Netflix Prize dataset (~77M ratings). Not included due to size.
