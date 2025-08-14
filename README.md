Release Note

Version 1.0.9.23:
Thêm log debug case fpt không add được thiết bị. vào hub là ir v2
Address luôn là 1 không lấy address từ api hoặc address từ hub trả về

- NGuyên nhân do nếu hub trước đó chưa có meshStatus giá trị do app chưa gọi api check status và lấy nextAddress ở bước check status thì ở bước add không có status và nextAddress
-> chủ động get lại status và nextAddress ở bước add
    

