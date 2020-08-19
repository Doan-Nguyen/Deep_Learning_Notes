# Chapter 1: Python Basics 


## Kiểu dữ liệu trong python 

+ Integer

+ Floating-Point

+ String

## Kết nối & mở rộng với String 

+ *string concatenation* có thể coi như phép cộng 2 string. Mở rộng ra *+* còn được dùng cho các kiểu dữ liệu khác, các thành phần trong phép cộng phải chung kiểu dữ liệu. 
```
>>> 'abc' + 123 # TypeError: 
>>> 'abc' + '123' # 'abc123' 
```

+ Ngoài ra, còn có thể chuyển đổi giữ các kiểu dữ liệu bằng hàm tương ứng với kiểu dữ liệu đó: 
    - int()
    - float()
    - str()

## Khởi tạo giá trị cho biến 

+ Cú pháp:
```
a = 4
```

## Tiêu chuẩn code PEP-8 

+ Đặt tên:
    - Hàm: my_function(), good_function()
    - Biến: x, src_img, dst_folder 
    - Lớp: BasicBlock(), MyClass()

+ Dòng trống:
    - Khoảng cách giữa 2 class nên là 2 dòng trống.
    - Khoảng cách giữa 2 hàm trong cùng class nên là 1 dòng trống.
    - Code trong 1 hàm không quá dài & nên chia <5 dòng thành một khối.

    ```
    import cv2 


    class FisrtClass():
        pass 


    class SecondClass():
        def first_method():
            pass 
        
        def second_method():
            pass 
    ```

+ Đóng ngoặc:
    ```
    list_of_numb = [
        1, 2, 3, 
        4, 5, 6, 
        7, 8, 9
    ]
    ```


# 2. Flow control

## Boolean Values & Boolean Operators

```
False != True
True and True
```

## *if, else, elif* Statements
```
if a < 12:
    print("Condition 1")
elif a >= 12 and a < 20:
    print("Condition 2)
else:
    print("Other")
```
