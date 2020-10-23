# Gradient Descent Optimization Algorithms

+ Tối ưu trong học máy quan tâm đến kết quả đo lường hiệu suất mô hình (P), được thực hiện trên tập test.
+ Quá trình tối ưu P dựa trên việc tối ưu cost function $J(\theta)$

## 1. Hàm tối ưu 
+ Hàm tối ưu còn được gọi là cost function, loss function ... Mục tiêu là tìm giá trị nhỏ nhất/lớn nhất cho hàm số.
+ Hai khái niệm cần quan tâm:
    - **Gradient**: được hiểu là đạo hàm bậc một của phương trình đa biến/xét trong không gian nhiều chiều.
    -  **Hessian**: đạo hàm bậc 2 của ma trận.

        ![Gradient Hessian](figures/gradient_hessian.png)

+ Đạo hàm từng phần bậc 2 (Second partial derivative)
    - Xét hàm $f$ đa biến
    - Stationary points (điểm dừng/cực trị): tại đó $\nabla f =0$
    - Sử dụng đạo hàm bậc 2 để kiểm thử:
        - Cứ nhớ đến bài đồ thị hàm số khi thi đại học ý.
    - Saddle point (điểm yên ngựa): tại đó Hessian đạt cả gía trị âm & giá trị dương. Hình minh họa:

        ![Saddle point](figures/saddle_point.png) 
## 2. Những thuật toán tối ưu cơ bản & han chế 

### 2.1 Batch Gradient Descent: quá trình.

    $\theta := \theta - \eta \nabla_\theta J(\theta)$

    - Khởi tạo kích thước bước nhảy (vận tốc)
    - Lựa chọn ngẫu nhiên điểm $\theta$
    - Tính toán đạo hàm $\nabla_\theta J(\theta)$ tại điểm $\theta$
    - Cập nhật giá trị $\theta$ đến mức ngưỡng nhỏ nhất mong muốn.

+ Đánh giá:
    - Nhược điểm: 
        - Cần tính toán đạo hàm cho **toàn bộ dữ liệu** 
        - Tốc độ tính toán chậm nếu không thực thi tối ưu.
    - Ưu điểm:
        - Hội tụ ổn định.

### 2.2 Stochastic Gradient Descent 
+ Tương tự Gradient Descent nhưng tại một thời điểm, ta **chỉ cập nhật** $\theta$ của hàm mất mát tại **chỉ một điểm dữ liệu** 
    - Một **epochs**: một lần duyệt qua tất cả các điểm trên toàn bộ dữ liệu -> mỗi epochs tương đương với một lần cập nhật $\theta$
    - Với SGD, mỗi epochs sẽ có *n* lần cập nhật $\theta$ với *n* là số điểm dữ liệu.
+ Cập nhật giá trị $\theta$:
    - Sau mỗi epoch, ta cần *shuffle* thứ tự các điểm dữ liệu để đảm báo tính ngẫu nhiên.
    - $\theta := \theta - \eta \nabla_\theta J(\theta; x_i; y_i)$
        - $J(\theta; x_i; y_i)$: hàm mất mát với chỉ một cặp điểm dữ liệu (input, label)

+ Đánh giá:
    - Ưu điểm:
        - Tốc độ hội tụ nhanh hơn *Batch Gradient Descent*
        - Hiệu quả khi học 'online' ~ khi cần cập nhật thêm dữ liệu, chỉ cần học thêm sẽ đạt hội tụ.
    - Nhược điểm:
        - Hội tụ không ổn định.
        - Không sử dụng các cách thức tối ưu vector


## 3. Thách thức trong việc tối ưu gradient descent

## 4. Luyện tập gradient descent
