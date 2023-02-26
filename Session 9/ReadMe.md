# Assignment Submission for Session 9

## The Dawn of Transformers

## Goals
1. Create custom model with ultimus module (that contains keys, queries and values matrices)
2. Use CIFAR dataset
3. Train model for 24 epochs using ADAM as optimizer

## Custom Model Summary
----------------------------------------------------------------
        Layer (type)               Output Shape         Param #
================================================================
            Conv2d-1           [-1, 32, 30, 30]             864
              GELU-2           [-1, 32, 30, 30]               0
       BatchNorm2d-3           [-1, 32, 30, 30]              64
            Conv2d-4          [-1, 256, 28, 28]          73,728
              GELU-5          [-1, 256, 28, 28]               0
       BatchNorm2d-6          [-1, 256, 28, 28]             512
            Conv2d-7           [-1, 48, 26, 26]         110,592
              GELU-8           [-1, 48, 26, 26]               0
       BatchNorm2d-9           [-1, 48, 26, 26]              96
AdaptiveAvgPool2d-10             [-1, 48, 1, 1]               0
           Linear-11                    [-1, 8]             392
           Linear-12                    [-1, 8]             392
           Linear-13                    [-1, 8]             392
          Softmax-14                    [-1, 8]               0
           Linear-15                   [-1, 48]             432
          Ultimus-16                   [-1, 48]               0
           Linear-17                    [-1, 8]             392
           Linear-18                    [-1, 8]             392
           Linear-19                    [-1, 8]             392
          Softmax-20                    [-1, 8]               0
           Linear-21                   [-1, 48]             432
          Ultimus-22                   [-1, 48]               0
           Linear-23                    [-1, 8]             392
           Linear-24                    [-1, 8]             392
           Linear-25                    [-1, 8]             392
          Softmax-26                    [-1, 8]               0
           Linear-27                   [-1, 48]             432
          Ultimus-28                   [-1, 48]               0
           Linear-29                    [-1, 8]             392
           Linear-30                    [-1, 8]             392
           Linear-31                    [-1, 8]             392
          Softmax-32                    [-1, 8]               0
           Linear-33                   [-1, 48]             432
          Ultimus-34                   [-1, 48]               0
           Linear-35                   [-1, 10]             490
================================================================
Total params: 192,778
Trainable params: 192,778
Non-trainable params: 0
----------------------------------------------------------------

## Training and Test Loss Charts

## Training Logs


