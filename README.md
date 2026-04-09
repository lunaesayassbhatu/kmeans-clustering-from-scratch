# K-Means Clustering from Scratch

A pure NumPy implementation of K-Means clustering supporting three distance metrics, benchmarked against ground-truth labels on a real dataset.

## What's Implemented

- **K-Means algorithm** built from scratch — no sklearn
- **Three distance metrics:**
  - Euclidean distance (vectorized with matrix ops)
  - Cosine distance
  - Jaccard distance
- **Cluster evaluation** using majority-vote accuracy and SSE (Sum of Squared Errors)
- **Comparison plots** — SSE and accuracy across all three metrics

## Results

| Metric | SSE | Accuracy |
|--------|-----|----------|
| Euclidean | lowest | competitive |
| Cosine | moderate | competitive |
| Jaccard | highest | varies |

## Project Structure

```
kmeans-clustering-from-scratch/
├── kmeans_clustering.ipynb   # Main notebook
├── data/
│   ├── data.csv              # Feature matrix
│   └── label.csv             # Ground truth labels
├── task1_outputs/
│   ├── task1_sse_vs_metric.png
│   └── task1_accuracy_vs_metric.png
└── requirements.txt
```

## Usage

```bash
pip install -r requirements.txt
jupyter notebook kmeans_clustering.ipynb
```

## Tech Stack

- Python
- NumPy
- pandas
- Matplotlib
