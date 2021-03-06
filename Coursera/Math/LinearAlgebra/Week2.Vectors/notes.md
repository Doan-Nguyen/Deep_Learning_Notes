# Finding the size of a vector, it's angle & projection

## Modules & inner product

+ Length of a vector:
    - r = a*i + b*j
    ![Length of a vector](figures/modulus_inner.png)

+ Product vectors:  
    ![Product of a vector](figures/multi.png)

## Cosine & dot product

+ Cosine rule:

    ![Cosine rule](figures/consine_rule.png)

    - Transform to vectors:  
    
    ![Transform to vectors](figures/transforms.png)


# Changing the reference frame

## Changing basis

+ Thay các đơn vị i, j bằng các ma trận đơn vị *e_1=(1, 0)*, *e_2=(0, 1)*. Biểu diễn bất kì vector bằng các ma trận đơn vị.

![Changing basic](figures/changing_basic1.png)

+ Xét hệ các vectors: V = {v1, v2, v3, ...}
    - Hệ các vector phụ thuộc tuyến tính khi và chỉ khi:
        ``` 
        k1*v1 + k2*v2 + ... = 0 | k*i* không đồng thời bằng 0
        ```
    - Hệ các vector độc lập tuyến tính khi và chỉ khi: 
        ```
        k1*v1 + k2*v2 + ... = 0 | chỉ có nghiệm duy nhất: k1=k2=k3=..=kn=0
        ```

+ 