# UART
1,Ý tưởng:

goc.txt là file text ngẫu nhiên 18kb

UART1: RX:PA10

       TX:PA9

UART2: RX:PA3

       TX:PA2

PB1: gửi dữ liệu đi

STM thứ nhất có tác dụng gửi dữ liệu bấm là PB1 gửi dữ liệu từ UART1 của STM1 đến UART1 của STM2

STM thứ hai có tác dụng nhận dữ liệu từ STM1 và bấm nút PB1 để gửi lên máy tính bằng UART2 thông qua USB-TTL

2,Nhận dữ liệu và phân tích:

Sau khi cài xong ultra-serial-port thì cài để đọc dữ liệu ghi vào file nhan.txt

coppy 2 file txt lên Unititle6 để so sánh 2 file text khác nhau bao nhiêu?

3,Lưu ý rằng khi thực hiện thì text của file nhan.txt sẽ mất những gói tin đoạn đầu.
 Hiện tại stm đen đang gửi
 stm đỏ đang nhận và gửi lên laptop

4, Các bước cần làm:

a,nối qua RS232 và thử nghiệm với các độ dài khác nhau, hãy thay đổi baudrate

b,lên dùng oscillo đo dạng sóng và dự đoán ảnh hưởng của oscicllo lên dạng sóng nếu không đo

c, dùng các nguồn khác nhau để cấp điện stm32

d, dùng các môi trường khác nhau : dây thẳng, cong, ngâm trong nước, hai sợi dây liền nhau, hai sợi dây tách nhau,...

5, Các ứng dụng cần cài: ultra-serialport, Keil-c, driver cho USB-TTL

6,Slide:
Các dụng cụ chuẩn bị
Bước thí nghiệm
Điều kiện thí nghiệm
Kết quả
Lập bảng từng bước tăng tần số, khoảng cách
Quy trình thí nghiệm ra lưu đồ, setup cho lần đầu chỉ là 1,2 byte pass thì mới truyền chuỗi byte.


link:
https://husteduvn-my.sharepoint.com/:f:/g/personal/phuoc_dh213723_sis_hust_edu_vn/EqgAfzQQAg1AvRDWQw9TUB8BoJUbUf6sXVP2JyAcwM-NCg?e=HrvUUi : Link đầy đủ hơn xíu

https://www.youtube.com/watch?v=PVOxgKheHsY  : Fix lỗi USB-TTL

https://www.youtube.com/watch?v=esIyBaXr_HE&t=1053s : truyền UART

https://www.youtube.com/watch?v=OQdwaZ1mIXA&t=648s : nhận UART-1

https://www.youtube.com/watch?v=pK4p__u2oHg : nhận UART-2

https://www.youtube.com/watch?v=bl6BjCr11vo&t=274s : tạo project với CubeMX

