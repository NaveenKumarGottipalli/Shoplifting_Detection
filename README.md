# Shoplifting_Detection — Multi-Model Shoplifting Detection Benchmark

## Overview
- **Project 1 (3D CNNs)**: `R(2+1)D` Baseline vs. `DMD-A-Net` (Frame-Differential Motion Gate + Temporal Concealment Cross-Attention)
- **Project 2 (Video Transformers)**: `TimeSformer` Baseline vs. `TCA-ViT` (Motion-Salience Patch Gate + Occlusion Gradient Head)
- **Project 3 (Skeleton Graph CNNs)**: `ST-GCN` vs. `CTR-GCN` vs. `VDA-GCN` (Velocity-Gated Temporal Conv + Directed Concealment Adjacency)

## Cross-Dataset Evaluation Plan (`NaveenKumarGottipalli/Shoplifting_DataCollection`)
- **Training & Validation Corpus**: `S3` + `Shop DataSet` + `UCF-Crime` (S1 removed)
- **Unseen Real-World Test Set**: `DCSASS Dataset` (`DCSASS Dataset/Labels/Shoplifting.csv`)

## Repository Structure
- `dataset_splits/`: Verified sample manifests (`train.json`, `val.json`, `test.json`, `quarantined.json`) and dataset visualizations
- `Project_1_R2Plus1D_DMD_ANet/`: `results/` JSONs, `figures/` (`confusion_matrix.png`, `accuracy_curve.png`, `roc_curve.png`, `input_vs_output_predictions.png`), and `figures/limitations/` (14 limitation studies)
- `Project_2_TimeSformer_TCA_ViT/`: `results/` JSONs, `figures/` (`confusion_matrix.png`, `accuracy_curve.png`, `roc_curve.png`, `input_vs_output_predictions.png`), and `figures/limitations/` (15 limitation studies)
- `Project_3_Skeleton_GCNs/`: `results/` JSONs, `figures/` (`confusion_matrix.png`, `accuracy_curve.png`, `roc_curve.png`, `input_vs_output_predictions.png`), and `figures/limitations/` (8 limitation studies)
- `All_Projects_Comparison/`: Cross-project summary tables and comparative charts
