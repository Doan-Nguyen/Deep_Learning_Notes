#   Tìm hiểu về các thuật toán sử dụng trong quá trình tiền xử lý ảnh 

Trong các dự án Computer Vision, bước tiền xử lý dữ liệu đóng vai trò rất quan trọng. Qua quá trình này, người kĩ sư có thể đánh giá chất lượng dữ liệu còn có thể cải thiện chất lượng, tăng sinh tập dữ liệu học cho mô hình. Trong bài viết này, mình muốn tìm câu trả lời "Tại sao sử dụng thuật toán (?) này ở bước này ?". Deeper !!!

## 1. Tại sao cần chuyển đổi ảnh RGB sang ảnh gray
+ Ảnh gray: ảnh đơn săc, mỗi giá trị điểm ảnh nằm trong khoảng [0, 255] tương ứng với 256 mức xám. Giá trị 0 - màu đen, giá trị 255 - màu trắng.
    - Ngưỡng xám (threshold): để tạo ra ảnh nhị phân từ ảnh xám ta cần lựa chọn mức ngưỡng "tốt nhất" để phân loại thành 2 nhóm: các điểm ảnh có giá trị quan tâm & các điểm ảnh có giá trị ít quan tâm.
    - Ảnh nhị phân (binary image): mỗi điểm ảnh biểu diễn chỉ bởi 2 giá trị: {0: trắng; 1: đen}.

+ Ý nghĩa việc convert ảnh RGB sang ảnh gray:
    - Ảnh xám sẽ giảm các thông tin không cần thiết như cường độ sáng, màu sắc trên ảnh gốc. 
    - Trên ảnh RGB, 3 kênh màu mang nhiều thông tin nhưng tương tự nhau trên các kênh. Việc giảm xuống 1 kênh màu giúp tăng tốc độ tính toán nhưng vấn giữ được các thông tin cần thiết.