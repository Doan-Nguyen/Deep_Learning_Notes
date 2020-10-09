# Convolutional and Cross correlation

+ Thuật toán áp dụng trong CNN là **cross correlation** chứ không phải *convolutional*.


## Sơ lược về Cross Correlation
+ Correlation là phép biến đổi mà ta áp dụng của sổ trượt trên ảnh gốc với phép biến đổi tích vô hướng **dot product**.
    - **dot product**: 
         $\vec{a}.\vec{b} = \sum^n_(i=1)a_i.b_i = a_1b_1 + a_2b_2 + ... + a_nb_n$
    - Tích vô hướng là tích của độ lớn vector & độ lớn phép chiếu vô hướng (vuông góc) của vector còn lại lên nó.
    - Kết quả của tính vô hướng thể hiện tương quan về hướng & độ lớn giữa 2 vector.
        - Giá trị tích vô hướng < 0 => 2 vector ngược hướng
        - Độ lớn tích vô hướng thể hiện độ lớn của 1 trong 2 vector rất lớn hoặc độ lớn hình chiều vector này lên vector kia rất lớn.
+ Source code *source.ipynb*


## Sơ lược về Convolutional
+ Convolutional được áp dụng nhiều trong Computer Vision. Có thể kể đến như các thuật toán làm mờ (blurring), làm mịn (smoothing) hoặc tìm cạnh đường biên (edge detection), tăng độ sắc nét (sharpen).
+ Convolution bản chất là ta xoay cửa sổ filter $180^o$, rồi sử dụng phép *correlation*.
+ Source code *source.ipynb*


## Tài liệu tham khảo:
[Convolution - Tích chập giải thích bằng code thực tế](https://techmaster.vn/posts/35474/convolution-tich-chap-giai-thich-bang-code-thuc-te)
[Bài giảng lớp INT3121-20 - cô Nguyen Thi Ngoc Diep](https://github.com/chupibk/INT3121-20/blob/master/week4/week%204%20-%20augmentation%20and%20generator.pdf)
[Convolutions with OpenCV and Python](pyimagesearch.com/2016/07/25/convolutions-with-opencv-and-python/)