#ThucHanhJMeter

# Kiểm tra hiệu năng trang web
# Mục tiêu:
- Sử dụng jMeter để tạo một kịch bản kiểm tra mô phỏng người dùng truy cập trang web https://thoitiet.vn/
- Chạy kịch bản kiểm tra và ghi lại kết quả.
- Phân tích kết quả kiểm tra, bao gồm thời gian phản hồi, số lượng yêu cầu thành công, số lượng yêu cầu thất bại, v.v.
- Dựa trên kết quả phân tích, đưa ra kết luận về hiệu năng của trang web.

# Kịch bản kiểm tra:
- Thread Group:
    + Số lượng thread: 100
    + Thời gian chạy: 60 giây
    + Ramp-up period: 10 giây
- HTTP Request:
    + URL: https://thoitiet.vn/
    + Method: GET
    + Content encoding: UTF-8
- Listeners:
    + View Results Tree
    + Aggregate Report

# Kết quả kiểm tra:
![image](https://github.com/tungsoi123/TH_Jmeter/assets/124906792/ac4a837c-eabe-440a-aac4-b73b06ecfe30)
![image](https://github.com/tungsoi123/TH_Jmeter/assets/124906792/d237aa51-a547-458f-ac0a-9b7f86f72de8)
![image](https://github.com/tungsoi123/TH_Jmeter/assets/124906792/7cfbe375-e6cc-4eee-8c6d-6450b26682df)

- Phân tích kết quả kiểm tra:
- Số lượng yêu cầu thành công: 100/100 = 100%
- Số lượng yêu cầu thất bại: 0/100 = 0%
- Thời gian phản hồi trung bình: 19,29 ms
- Thời gian phản hồi trung vị: 21,49 ms
- Thời gian phản hồi percentil 90: 23,50 ms
- Chuyển tải:  yêu cầu/giây
# Kết luận:
Trang web https://thoitiet.vn/ có hiệu năng khá tốt. Số lượng yêu cầu thành công rất cao (100%), số lượng yêu cầu thất bại thấp (0%). Thời gian phản hồi trung bình, trung vị và percentil 90 đều ở mức thấp (trên dưới 100 ms). Chuyển tải của trang web ở mức trung bình ( yêu cầu/giây).


# Kiểm tra hiệu năng API
# Mục tiêu:
- Sử dụng jMeter để tạo một kịch bản kiểm tra mô phỏng người dùng truy cập API https://reqres.in/api/login
- Chạy kịch bản kiểm tra và ghi lại kết quả.
- Phân tích kết quả kiểm tra, bao gồm thời gian phản hồi, số lượng yêu cầu thành công, số lượng yêu cầu thất bại, v.v.
- Dựa trên kết quả phân tích, đưa ra kết luận về hiệu năng của API.
  
# Kịch bản kiểm tra:
- Thread Group:
    + Số lượng thread: 100
    + Thời gian chạy: 60 giây
    + Ramp-up period: 10 giây
- HTTP Request:
    + URL: https://reqres.in/api/login
    + Method: POST
    + Content encoding: UTF-8
- Listeners:
    + View Results Tree
    + Aggregate Report
      
# Kết quả kiểm tra:
![image](https://github.com/tungsoi123/TH_Jmeter/assets/124906792/d712d970-0ea4-425b-94a2-5f1c9c92edc1)
![image](https://github.com/tungsoi123/TH_Jmeter/assets/124906792/314b3982-5b9e-41f8-872a-93f8d517cba1)
![image](https://github.com/tungsoi123/TH_Jmeter/assets/124906792/a6cd2d1f-6520-4bf6-9116-8eb86ace7bda)

- Phân tích kết quả kiểm tra:
- Số lượng yêu cầu thành công: 100/100 = 100%
- Số lượng yêu cầu thất bại: 0/100 = 0%
- Thời gian phản hồi trung bình: 15,08 ms
- Thời gian phản hồi trung vị: 14,32ms
- Thời gian phản hồi percentil 90: 14,77 ms
- Chuyển tải:  yêu cầu/giây
# Kết luận:
Trang web https://openweathermap.org/current có hiệu năng tốt. Số lượng yêu cầu thành công rất cao (100%), số lượng yêu cầu thất bại thấp (0%). Thời gian phản hồi trung bình, trung vị và percentil 90 đều ở mức thấp (dưới 100 ms). Chuyển tải của trang web ở mức tốt 

# So Sánh :

Với 2 trang web https://thoitiet.vn/ và https://reqres.in/api/login,thì https://reqres.in/api/login có hiệu năng tốt hơn khi có thể phản hồi số lượng request lớn hơn, tỉ lệ lỗi nhỏ hơn, thời gian phản hồi nhanh hơn
