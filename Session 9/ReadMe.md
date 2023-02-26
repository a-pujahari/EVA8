# Assignment Submission for Session 9

## The Dawn of Transformers

## Goals
1. Create custom model with ultimus module (that contains keys, queries and values matrices)
2. Use CIFAR dataset
3. Train model for 24 epochs using ADAM as optimizer


## Custom Model Summary
|       Layer (type)     |         Output Shape     |   Param # |
|------------------------|--------------------------|-----------|
|           Conv2d-1     |     [-1, 32, 30, 30]     |       864 |
|             GELU-2     |     [-1, 32, 30, 30]     |         0 |
|      BatchNorm2d-3     |     [-1, 32, 30, 30]     |        64 |
|           Conv2d-4     |    [-1, 256, 28, 28]     |    73,728 |
|             GELU-5     |    [-1, 256, 28, 28]     |         0 |
|      BatchNorm2d-6     |    [-1, 256, 28, 28]     |       512 |
|           Conv2d-7     |     [-1, 48, 26, 26]     |   110,592 |
|             GELU-8     |     [-1, 48, 26, 26]     |         0 |
|      BatchNorm2d-9     |     [-1, 48, 26, 26]     |        96 |
|AdaptiveAvgPool2d-10    |       [-1, 48, 1, 1]     |         0 |
|          Linear-11     |              [-1, 8]     |       392 |
|          Linear-12     |              [-1, 8]     |       392 |
|          Linear-13     |              [-1, 8]     |       392 |
|         Softmax-14     |              [-1, 8]     |         0 |
|          Linear-15     |             [-1, 48]     |       432 |
|         Ultimus-16     |             [-1, 48]     |         0 |
|          Linear-17     |              [-1, 8]     |       392 |
|          Linear-18     |              [-1, 8]     |       392 |
|          Linear-19     |              [-1, 8]     |       392 |
|         Softmax-20     |              [-1, 8]     |         0 |
|          Linear-21     |             [-1, 48]     |       432 |
|         Ultimus-22     |             [-1, 48]     |         0 |
|          Linear-23     |              [-1, 8]     |       392 |
|          Linear-24     |              [-1, 8]     |       392 |
|          Linear-25     |              [-1, 8]     |       392 |
|         Softmax-26     |              [-1, 8]     |         0 |
|          Linear-27     |             [-1, 48]     |       432 |
|         Ultimus-28     |             [-1, 48]     |         0 |
|          Linear-29     |              [-1, 8]     |       392 |
|          Linear-30     |              [-1, 8]     |       392 |
|          Linear-31     |              [-1, 8]     |       392 |
|         Softmax-32     |              [-1, 8]     |         0 |
|          Linear-33     |             [-1, 48]     |       432 |
|         Ultimus-34     |             [-1, 48]     |         0 |
|          Linear-35     |             [-1, 10]     |       490 |
----------------------------------------------------------------
Total params: 192,778

Trainable params: 192,778 

Non-trainable params: 0 


## Training and Test Loss Charts

![LossGraphs](https://user-images.githubusercontent.com/31046307/221427858-a0793cee-b0f1-4f19-8a2d-cc24b5c3b2b6.png)


## Training Logs
EPOCH: 1
Loss=1.0537220239639282 Batch_id=97 LR=0.00085 Accuracy=54.65: 100%|█| 98/98 [00

Test set: Average loss: 0.0024, Accuracy: 5346/10000 (53.46%)

EPOCH: 2
Loss=1.1473230123519897 Batch_id=97 LR=0.00242 Accuracy=55.81: 100%|█| 98/98 [00

Test set: Average loss: 0.0025, Accuracy: 5369/10000 (53.69%)

EPOCH: 3
Loss=1.324575662612915 Batch_id=97 LR=0.00431 Accuracy=48.50: 100%|█| 98/98 [00:

Test set: Average loss: 0.0027, Accuracy: 4590/10000 (45.90%)

EPOCH: 4
Loss=2.3139288425445557 Batch_id=97 LR=0.00572 Accuracy=31.61: 100%|█| 98/98 [00

Test set: Average loss: 0.0048, Accuracy: 821/10000 (8.21%)

EPOCH: 5
Loss=1.5903565883636475 Batch_id=97 LR=0.00610 Accuracy=24.98: 100%|█| 98/98 [00

Test set: Average loss: 0.0033, Accuracy: 3009/10000 (30.09%)

EPOCH: 6
Loss=1.2437877655029297 Batch_id=97 LR=0.00605 Accuracy=40.98: 100%|█| 98/98 [00

Test set: Average loss: 0.0027, Accuracy: 4903/10000 (49.03%)

EPOCH: 7
Loss=2.37015962600708 Batch_id=97 LR=0.00591 Accuracy=27.88: 100%|█| 98/98 [00:1

Test set: Average loss: 0.0049, Accuracy: 1087/10000 (10.87%)

EPOCH: 8
Loss=2.017784833908081 Batch_id=97 LR=0.00569 Accuracy=15.35: 100%|█| 98/98 [00:

Test set: Average loss: 0.0042, Accuracy: 1790/10000 (17.90%)

EPOCH: 9
Loss=1.9367401599884033 Batch_id=97 LR=0.00541 Accuracy=17.92: 100%|█| 98/98 [00

Test set: Average loss: 0.0040, Accuracy: 1962/10000 (19.62%)

EPOCH: 10
Loss=2.1714067459106445 Batch_id=97 LR=0.00506 Accuracy=22.61: 100%|█| 98/98 [00

Test set: Average loss: 0.0050, Accuracy: 1326/10000 (13.26%)

EPOCH: 11
Loss=2.200700044631958 Batch_id=97 LR=0.00466 Accuracy=21.29: 100%|█| 98/98 [00:

Test set: Average loss: 0.0042, Accuracy: 1761/10000 (17.61%)

EPOCH: 12
Loss=1.8507556915283203 Batch_id=97 LR=0.00422 Accuracy=19.84: 100%|█| 98/98 [00

Test set: Average loss: 0.0037, Accuracy: 2262/10000 (22.62%)

EPOCH: 13
Loss=1.8833717107772827 Batch_id=97 LR=0.00374 Accuracy=25.35: 100%|█| 98/98 [00

Test set: Average loss: 0.0036, Accuracy: 2765/10000 (27.65%)

EPOCH: 14
Loss=1.6621544361114502 Batch_id=97 LR=0.00325 Accuracy=32.43: 100%|█| 98/98 [00

Test set: Average loss: 0.0033, Accuracy: 3528/10000 (35.28%)

EPOCH: 15
Loss=1.518742322921753 Batch_id=97 LR=0.00275 Accuracy=37.63: 100%|█| 98/98 [00:

Test set: Average loss: 0.0031, Accuracy: 3744/10000 (37.44%)

EPOCH: 16
Loss=1.780297040939331 Batch_id=97 LR=0.00226 Accuracy=28.99: 100%|█| 98/98 [00:

Test set: Average loss: 0.0036, Accuracy: 2679/10000 (26.79%)

EPOCH: 17
Loss=1.7211952209472656 Batch_id=97 LR=0.00179 Accuracy=30.17: 100%|█| 98/98 [00

Test set: Average loss: 0.0034, Accuracy: 3471/10000 (34.71%)

EPOCH: 18
Loss=1.676878809928894 Batch_id=97 LR=0.00135 Accuracy=31.46: 100%|█| 98/98 [00:

Test set: Average loss: 0.0034, Accuracy: 3518/10000 (35.18%)

EPOCH: 19
Loss=1.535071611404419 Batch_id=97 LR=0.00096 Accuracy=37.66: 100%|█| 98/98 [00:

Test set: Average loss: 0.0031, Accuracy: 3833/10000 (38.33%)

EPOCH: 20
Loss=1.5658873319625854 Batch_id=97 LR=0.00063 Accuracy=40.11: 100%|█| 98/98 [00

Test set: Average loss: 0.0030, Accuracy: 3994/10000 (39.94%)

EPOCH: 21
Loss=1.4804667234420776 Batch_id=97 LR=0.00036 Accuracy=41.66: 100%|█| 98/98 [00

Test set: Average loss: 0.0030, Accuracy: 4043/10000 (40.43%)

EPOCH: 22
Loss=1.4399409294128418 Batch_id=97 LR=0.00016 Accuracy=42.04: 100%|█| 98/98 [00

Test set: Average loss: 0.0039, Accuracy: 3908/10000 (39.08%)

EPOCH: 23
Loss=1.4467012882232666 Batch_id=97 LR=0.00004 Accuracy=42.44: 100%|█| 98/98 [00

Test set: Average loss: 0.0030, Accuracy: 4118/10000 (41.18%)

EPOCH: 24
Loss=1.469463586807251 Batch_id=97 LR=0.00000 Accuracy=42.50: 100%|█| 98/98 [00:

Test set: Average loss: 0.0030, Accuracy: 4121/10000 (41.21%)
