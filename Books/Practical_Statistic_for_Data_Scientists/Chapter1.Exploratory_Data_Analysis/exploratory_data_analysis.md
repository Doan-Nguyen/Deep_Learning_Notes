# Chương 1. Khám phá phân tích dữ liệu 


## 1.1 Thành phần của dữ liệu dạng cấu trúc 

+ Dữ liệu đến từ nhiều nguồn khác nhau như: các thông số thiết bị đo đạc, các sự kiện, text, ảnh, video .... Dữ liệu có thể chia thành: dữ liệu cấu trúc & dữ liệu phi cấu trúc. 
+ Khái niệm dữ liệu cấu trúc & phi cấu trúc mình xin trích dẫn theo bài viết trên tạp chí "Tia Sáng" [link bài viết](https://tiasang.com.vn/khoa-hoc-cong-nghe/Khai-thac-du-lieu-phi-cau-truc-12346). Theo đó:
    - Dữ liệu phi cấu trúc là những thông tin không được định nghĩa từ trước về mô hình dữ liệu hay cách tổ chức nôi dung dữ liệu. Có thể kể đến như: hình ảnh, text, chuỗi sự kiện/hành vi của user trên 1 trang web.
    - Dữ liệu cấu trúc: thường là các tệp văn bản, thông tin được hiển thị trong các cột & hàng. Có 2 kiểu dữ liệu cơ bản là:
        - Số:
            - Rời rạc: dữ liệu được lấy tại một thời điểm nhất định. vd: khoảng thời gian, số, số thập phần
            - Liên tục: dữ liệu chỉ tồn tại dạng số nguyên.
        - Tiêu đề/loại dữ liệu:
            - Binary: Chỉ tồn tại 2 trạng thái của catogories: 0/1
            - Ordinal: Thể hiện cụ thể thông tin.

## 1.2 Dữ liệu kiểu bảng 
+ Thường xuất hiện dưới dạng bảng hoặc spreadsheet. Khuôn mẫu chung có kiểu dữ liệu dạng này là ma trận 2 chiều:
    - Cột dọc: thể hiện các đặc trưng/biến chung của các đối tượng thể hiện trong bảng.
    - Hàng ngang: thể hiện các trường hợp/đối tượng được phân tích.
+ Đặc trưng quan trọng thường xuất hiện:
    - Data frame: 