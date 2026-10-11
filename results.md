# Cats vs Dogs Dataset
1.
For  parameters:
` EPOCHS, BATCH_SIZE, IMAGE_SIZE = 100, 32, 128
TREE_DEPTH, FEATURE_SIZE, NODE_HIDDEN_SIZE = 1, 128, 32
LEARNING_RATE, VAL_FRACTION, SEED = 1e-3, .2, 42 `

`Metric	Result
First epoch with 100% training accuracy	77
Best validation accuracy	82.95%
Epoch of best validation accuracy	90
Total epochs completed	113
Architecture	Shared CNN + depth-1 soft tree`

<img width="1798" height="861" alt="image" src="https://github.com/user-attachments/assets/6c66b4b4-c5a8-4217-b5dc-eeb9d1a5bbbe" />


2.
For parameters:
`EPOCHS, BATCH_SIZE, IMAGE_SIZE = 100, 32, 96
TREE_DEPTH, FEATURE_SIZE, NODE_HIDDEN_SIZE = 1, 64, 16
LEARNING_RATE, VAL_FRACTION, SEED = 1e-3, .2, 42`

`Metric Result
First epoch with 100% training accuracy	68
Best validation accuracy	84.63%
Epoch of best validation accuracy	62
Total epochs completed	100
Architecture	Shared CNN + depth-1 soft tree`

Trainable parameters: 390,469
<img width="1489" height="490" alt="image" src="https://github.com/user-attachments/assets/d3a32631-1ac6-457c-9785-78f812a6edc1" />
