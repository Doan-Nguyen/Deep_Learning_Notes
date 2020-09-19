# Run Length Encode


## Run Length Encoder ~ thuật toán nén dữ liệu 
+ Thuật toán để mô tả các dữ liệu mang tính chất lặp đi lặp lại. Trong bài toán *segmentation*, các điểm ảnh có giá trị pixel là 1 sẽ được mã hóa.
+ Chuỗi encoded có dạng string:
    ```
    start, length, start, length ...
    ```
    - (start, length): sẽ thể hiện 1 đoạn line trong tập hợp các đoạn line cấu thành đường biên vùng segmentation.
