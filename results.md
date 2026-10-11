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



# CIFAR 10

PROFILE : SMOKE
`"smoke": dict(epochs=3, train_samples=4000, val_samples=1000, batch_size=128,
                  feature_size=32, hidden_size=8, depth=2, lr=2e-3)`

 `cap_f16_h4_d1: epoch 1/8
  batch   1/24
  train acc 0.120, val acc 0.133, val loss 2.294 | 10.3s/epoch
cap_f16_h4_d1: epoch 2/8
  batch   1/24
  train acc 0.156, val acc 0.177, val loss 2.222 | 9.5s/epoch
cap_f16_h4_d1: epoch 3/8
  batch   1/24
  train acc 0.175, val acc 0.179, val loss 2.141 | 8.8s/epoch
cap_f16_h4_d1: epoch 4/8
  batch   1/24
  train acc 0.180, val acc 0.195, val loss 2.091 | 8.7s/epoch
cap_f16_h4_d1: epoch 5/8
  batch   1/24
  train acc 0.189, val acc 0.170, val loss 2.050 | 8.6s/epoch
cap_f16_h4_d1: epoch 6/8
  batch   1/24
  train acc 0.200, val acc 0.187, val loss 1.985 | 8.5s/epoch
cap_f16_h4_d1: epoch 7/8
  batch   1/24
  train acc 0.199, val acc 0.176, val loss 1.993 | 8.5s/epoch
cap_f16_h4_d1: epoch 8/8
  batch   1/24
  train acc 0.203, val acc 0.196, val loss 1.931 | 8.4s/epoch
cap_f32_h8_d2: epoch 1/8
  batch   1/24
  train acc 0.124, val acc 0.214, val loss 2.107 | 8.8s/epoch
cap_f32_h8_d2: epoch 2/8
  batch   1/24
  train acc 0.206, val acc 0.263, val loss 1.981 | 9.0s/epoch
cap_f32_h8_d2: epoch 3/8
  batch   1/24
  train acc 0.232, val acc 0.265, val loss 1.904 | 8.6s/epoch
cap_f32_h8_d2: epoch 4/8
  batch   1/24
  train acc 0.257, val acc 0.286, val loss 1.882 | 9.1s/epoch
cap_f32_h8_d2: epoch 5/8
  batch   1/24
  train acc 0.288, val acc 0.281, val loss 1.815 | 9.0s/epoch
cap_f32_h8_d2: epoch 6/8
  batch   1/24
  train acc 0.300, val acc 0.282, val loss 1.800 | 9.0s/epoch
cap_f32_h8_d2: epoch 7/8
  batch   1/24
  train acc 0.308, val acc 0.325, val loss 1.738 | 9.1s/epoch
cap_f32_h8_d2: epoch 8/8
  batch   1/24
  train acc 0.326, val acc 0.329, val loss 1.733 | 9.0s/epoch
cap_f64_h16_d2: epoch 1/8
  batch   1/24
  train acc 0.142, val acc 0.184, val loss 2.083 | 8.2s/epoch
cap_f64_h16_d2: epoch 2/8
  batch   1/24
  train acc 0.209, val acc 0.240, val loss 1.985 | 8.5s/epoch
cap_f64_h16_d2: epoch 3/8
  batch   1/24
  train acc 0.231, val acc 0.272, val loss 1.932 | 8.2s/epoch
cap_f64_h16_d2: epoch 4/8
  batch   1/24
  train acc 0.264, val acc 0.263, val loss 1.876 | 8.3s/epoch
cap_f64_h16_d2: epoch 5/8
  batch   1/24
  train acc 0.283, val acc 0.289, val loss 1.844 | 8.5s/epoch
cap_f64_h16_d2: epoch 6/8
  batch   1/24
  train acc 0.302, val acc 0.287, val loss 1.829 | 8.4s/epoch
cap_f64_h16_d2: epoch 7/8
  batch   1/24
  train acc 0.298, val acc 0.297, val loss 1.761 | 8.4s/epoch
cap_f64_h16_d2: epoch 8/8
  batch   1/24
  train acc 0.313, val acc 0.347, val loss 1.741 | 8.4s/epoch
`


  
    
       
      feature_size
      hidden_size
      depth
      parameters
      train_accuracy
      validation_accuracy
      validation_error
    
  
  
    
      0
      16
      4
      1
      57669
      0.203
      0.196
      0.804
    
    
      1
      32
      8
      2
      60635
      0.326
      0.329
      0.671
    
    
      2
      64
      16
      2
      68491
      0.313
      0.347
      0.653
    
<img width="1386" height="207" alt="image" src="https://github.com/user-attachments/assets/312d589b-7eff-4184-bc0c-102dae72dc10" />
<img width="545" height="395" alt="image" src="https://github.com/user-attachments/assets/6d03a85e-52ff-4fde-a433-b569f81782de" />

No tested model reached 99% train accuracy; interpolation threshold was not observed.



 True class: cat  predicted: horse
Leaf reach probabilities: [0.299 0.1   0.359 0.242]
Leaf class predictions: ['deer', 'cat', 'truck', 'horse']
<img width="561" height="273" alt="image" src="https://github.com/user-attachments/assets/3c95d34b-0f9c-4452-a564-ede3e2468995" />
<img width="795" height="454" alt="image" src="https://github.com/user-attachments/assets/52ba977e-be50-4b8d-9bd9-408e81a5ca0c" />
The CNN has spatial receptive fields; routing MLPs consume the CNN feature vector. Saliency maps image regions that change a routing score.


<img width="968" height="393" alt="image" src="https://github.com/user-attachments/assets/a66d4bd9-4b0c-4e63-a9a2-d2e26047cadc" />
Training and validation curves for a 641,323-parameter soft neural tree trained on 1,000 CIFAR-10 images. Training accuracy reached 99.6%, while validation accuracy remained near 40% and validation loss increased substantially. The divergence demonstrates severe overfitting. The best-validation checkpoint achieved 41.2% test accuracy.


PROFILE: BASELINE
` "baseline": dict(epochs=25, train_samples=20000, val_samples=5000, batch_size=128,
                     feature_size=64, hidden_size=16, depth=2, lr=1e-3) `

<img width="981" height="393" alt="image" src="https://github.com/user-attachments/assets/96a0ec96-1c35-411a-882f-d7ab2718b32f" />
<img width="1388" height="499" alt="image" src="https://github.com/user-attachments/assets/c436f0a3-6226-44ee-bca2-c2eacb730bd0" />

Capacity / double descent experiment
<img width="1482" height="939" alt="image" src="https://github.com/user-attachments/assets/d2b99c37-08f3-414e-b11d-2ddb03c33bff" />
<img width="1711" height="1266" alt="image" src="https://github.com/user-attachments/assets/a6efb240-f820-4b77-8295-8756e2ecdc09" />
