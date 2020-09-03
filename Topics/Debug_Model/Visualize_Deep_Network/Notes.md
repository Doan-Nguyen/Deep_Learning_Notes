# Visualize Deep Network Models & Metric 

## TensorBoard
+ It is important to track every move & to examine results at each step.
+ TensorBoard on pytorch:
    - [Tutorials](https://pytorch.org/tutorials/intermediate/tensorboard_tutorial.html)

## Metrics (Loss & accuracy)

+ Using TensorBoard to record the accuracy & the cost function of model


# How to Unit test machine learning code

+ Hãy chắc chắn kiểm soát giá trị đầu vào, ngay cả khi bạn khởi tạo random tensor đầu vào, hãy xác định chúng.

+ Test các đơn vị nhỏ.

+ Hãy đảm bảo reset the graph giữa mỗi lần test.

## Sử dụng mltest 

+ Install: 
```
$ pip install mltest
```

+ Một vài nội dung được test:
    - Test sự thay đổi biến 
        - Sử dụng *train_op* & đảm bảo toàn bộ các biến đã được modified.
    
