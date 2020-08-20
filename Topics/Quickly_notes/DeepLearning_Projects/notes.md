# 1. Start a Deep Learning project

## Debug Deep Network (DN) is tough
+ Bắt đầu đơn giản & thay đổi dần dần.
+ Khi mô hình hoạt động, bắt đầu tối ưu. 
+ Mô hình hóa dự đoán & metrics của mô hình. 
+ *Start small, move small.*

## Measure & learn 
+ Thiết kế, lên đánh giá các bản kiểm thử & thực hiện ngay khi có thể 
+ Phân tích các lỗi sai.
+ *Build, measure & learn.*

## Time line 
+ Four phases with the last 3 phases executed in multiple iterations.
    - Project research 
    - Design 
    - Implementation & debug 
    - Experiment & tuning

+ Standing on the shoulders of giants
    - Skim through the paper quickly to grab the core ideas
    - Pay attention to the figures
    - What is important, read the paper again


# 2. Build a Deep learning datasets

## Dataset
+ *Garbage in & garbage out. Good data trains good models.*
+ To recap:
    - Use public dataset if possible
    - Find the best site(s) for high quality and diversify samples.
    - Categorize samples into folders. Merge data based on the lessons learned.
    - Analyze errors and filter out samples irrelevant to your real-life problem.
    - Balanced the number of samples for each class.
    - Shuffle your samples before training.
    - Collect sufficient samples. If not, apply transfer training.


# 3. Deep learning designs 

+ Simple and smart
    - Do not waste time training the model with too many iterations or too large batch size.

## Priority & incremental driven design:
- Break down complex problems into smaller problems and solve them in steps.
- Use shorter and smaller design iterations to make the project manageable

## Avoid random improvements
- Visualize the errors (badly performed scenarios) and the performance metrics to identify real issues

## Constraints
- Building deep learning is not only putting layers together.
- Apply constraints to the network design to make training more effective.
- *DL is more than adding layers*


# 4. Design details

## Deep learning software frameworks
+ If you want to train the model with multiple machines or deploy the inference engine onto a mobile phone, TensorFlow is the only choice.
+ **Pytorch convert Caffe2 using ONNX**
+ Suggest using pre-trained.

## Cost function 
+ Classification: Cross entropy, SVM 
+ Regression: Mean Square Error (MSE)
+ Object detection or segmentation: Intersection over Union (IoU)
+ Policy optimization: Kullback-Leibler divergence 
+ Word embedding: Noise Contrastive Estimation (NCE)
+ *Finding good cost functions becomes more important when we move into less familiar problem domains.*



# Summary 
```
+ Define task (Object detection, Colorization of line arts)
+ Collect dataset (MS Coco, Public web sites)
    ◦ Search for academic datasets and baselines
    ◦ Build your own (From Twitter, News, Website,…)
+ Define the metrics
    ◦ Search for established metrics
+ Clean and preprocess the data
    ◦ Select features and transform data 
    ◦ One-hot vector, bag of words, spectrogram etc...
    ◦ Bucketize, logarithm scale, spectrogram
    ◦ Remove noise or outliers 
    ◦ Remove invalid and duplicate data
    ◦ Scale or whiten data
+ Split datasets for training, validation and testing
    ◦ Visualize data
    ◦ Validate dataset
+ Establish a baseline
    ◦ Compute metrics for the baseline
    ◦ Analyze errors for area of improvements
+ Select network structure
    ◦ CNN, LSTM…
+ Implement a deep network
    ◦ Code debugging and validation
    ◦ Parameter initialization
    ◦ Compute loss and metrics
    ◦ Choose hyper-parameters
    ◦ Visualize, validate and summarize result
    ◦ Analyze errors
    ◦ Add layers and nodes
    ◦ Optimization
+ Hyper-parameters fine tunings
+ Try our model variants
```

# Reference:
+ https://medium.com/@jonathan_hui/deep-learning-designs-part-3-e0b15ef09ccc 