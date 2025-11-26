# Machine-Learning-Project---Christmas-Gift-Price-Prediction


K-Means Cluster Evaluation Metrics:

Elbow Method (Inertia vs k): Suggests k ≈ 5–6 (flattening of inertia curve).

Silhouette Score: Peaks at k = 2, indicating best cluster cohesion/separation.

Davies-Bouldin Index: Lowest at k ≈ 6, meaning clusters are compact and well-separated.

Takeaway:

Silhouette favors fewer, well-separated clusters (k = 2).

Elbow & DB index favor slightly more granular clusters (k = 5–6).

Choice depends on priority: simplicity vs. detailed structure.

Hierarchical Clustering Dendrogram:

Dendrogram suggests 2 main clusters, consistent with the Silhouette recommendation.

Overall Recommendation:

Simpler, cleaner clustering: k = 2 (supported by Silhouette and dendrogram).

More detailed grouping: k = 5–6 (supported by Elbow and DB index), but clusters are less distinct.
