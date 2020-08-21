# Debugging Strategies
*(page 431, "Deep Learning" - Ian Goodfellow and Yoshua Bengio)*

+ Machine learning systems are diﬃcult to debug for various reasons.

+ Some important debugging tests include the following:
    - **Visualize the model in action**
    - **Visualize the worst mistakes**
    - **Reason about software using training & testing error**
    - **Fit a tiny dataset**
    - **Compare back-propagated derivatives to numerical derivatives**
    - **Monitor histograms of activations and gradient**

## 1. Visualize the model in action (deploy)
+ This may seem obvious, but it is easy to fall into the practice of looking only at quantitative performance measurements like accuracy or log-likelihood.

## 2. Visualize the worst mistakes
+ Phần lớn các model sẽ trả về đầu ra là độ chính xác/ độ tin cậy cho dự đoán của model được sắp xếp tăng dần. 
+ Kết quả *maximum likelihood training* thường đáng tin cậy hơn xác suât độ chính xác dự đoán.  