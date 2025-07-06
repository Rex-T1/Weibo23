# Weibo23 Dataset (Update soon)
**Official repository for "MUPI: Rumor Detection Based on Multi-Entity and Multi-Relationship User-Post Interaction Networks"**

## Download Dataset
- The dataset can be download from [Google Drive](https://drive.google.com/file/d/1JqJ6ZrTwYDYwkcR2tws9AcOZJtNPEJSw/view?usp=sharing)

## Dataset Structure
```txt
├── label.csv                     # Class labels for all samples
│
├── event split/                  # Event-based dataset partition
│   ├── train.csv                 # Training set (events not in val/test)
│   ├── val.csv                   # Validation set
│   └── test.csv                  # Test set
│
├── time split/                   # Time-based dataset partition
│   ├── train_val.csv             # Weibo data before 2022
│   └── test.csv                  # Weibo data after 2022
│
├── weibo_original/               # Raw data and processing intermediates
│   ├── {weibo_id}-post.csv       # Original post content
│   ├── {weibo_id}-forwarding.csv # Original forwarding data
│   ├── {weibo_id}-comment.csv    # Original comment data
│   ├── {weibo_id}_user.csv       # Forwarding user information
│   ├── {weibo_id}_binary.csv     # Forwarding the binary feature of the user
│   ├── {weibo_id}_number.csv     # Forwarding the numerical feature of user
│   ├── {weibo_id}_onehot.csv     # Forwarding the one hot feature of the user
│   ├── {weibo_id}_text.csv       # Forwarding user text-like features
│   ├── {weibo_id}_graph.txt      # Forwarding graph
│   ├── {weibo_id}_number_graph.txt # Numerical encoding of the forwarding graph
│   ├── {weibo_id}_map.txt        # User name → ID mapping
│   ├── {weibo_id}_inverse_map.txt # ID → user name mapping
│   ├── {weibo_id}_text.json      # Ordinary forwarding text relationship graph
│   ├── {weibo_id}_special.json   # Specific forwarding text relationship graph
│   └── {weibo_id}_time.json      # Temporal propagation data
│
└── weibo_graph/                  # Processed datasets
    └── ...                       # (Additional processed files)
```
