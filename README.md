# Weibo23 (Update soon)
Official repository for "MUPI: Rumor Detection Based on Multi-Entity and Multi-Relationship User-Post Interaction Networks".
### Dataset
```txt
├── label.csv       Class tag file
├── event split/    A dataset divided by events
│ ├── train.csv
│ ├── val.csv
│ ├── test.csv
├── event split/    A dataset divided by time
│ ├── train_val.csv Weibo data before 2022
│ └── test.csv      Weibo data after 2022
├── weibo_original  Original data of Weibo and intermediate results of data processing
│─────| weibo_id ...
│     │── id-微博内容.csv Original post data
│     │── id-转发内容.csv Original forwarding data
│     │── id-评论内容.csv Original comment data
│     │── id_user.csv    Forwarding user information
│     │── id_binary.csv  Forwarding the binary feature of the user
│     │── id_number.csv  Forwarding the numerical feature of user
│     │── id_onehot.csv  Forwarding the one hot feature of the user
│     │── id_text.csv    Forwarding user text-like features
│     │── id_graph.txt   Forwarding graph
│     │── id_number_graph.txt  Numerical encoding of the forwarding graph
│     │── id_map.txt           The mapping from the user name to the encoding
│     │── id_inverse_map.txt   Reverse mapping from encoding to user name
│     │── id_text.json         Ordinary forwarding text relationship graph
│     │── id_special.json      Specific forwarding text relationship graph
│     │── id_time.json         Forwarding time relationship
├── weibo_graph ...      Processed datasets
```
