* Modeled MOOC interactions as a multi-relational heterograph (Student↔Enrollment↔Course) at scale (140K+ enrollments) and
built a consistent train/test ID + feature pipeline (numeric + time features, standardized).
* Implemented relation-aware message passing using DGL HeteroGraphConv (GraphSAGE) with learned entity embeddings and an
enrollment-level dropout classifier head.
* Improved learning under extreme class imbalance via pos weight in BCEWithLogitsLoss and validated with AUC/AUPRC; enabled
GPU training + batch inference to output dropout probabilities.
