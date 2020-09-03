# Pytorch Performance Tuning Guide

## Enable Async Data Loading & Augmentation
+ If num_workers > 0 to enable asynchronous data process:
    - num_workers = 4.number_GPU

+ Config: 
    - pin_memory = True

## Increase Batch Size
+ Increase batch_size to max out GPU memory
+ When increase batch size:
    - tune learning rate, add learning rate warmup & learning rate decay

## Disable bias for convolutions directly followed by a Batch Norm
+ Recommend:
    - [nn.Conv2d(..., bias=False, ...) -> nn.BatchNorm2d()]
