# 23640471_TranHoThuHuong_cabsystem
1. Vấn đề của hệ thống:
   Hệ thống đặt xe hiện tại còn nhiều hạn chế trong việc phân công tài xế, theo dõi chuyến đi, quản lý thanh toán và vận hành. Hệ thống khó mở rộng, thiếu tự động hóa
   và chưa đáp ứng tốt nhu cầu quản lý, bảo mật và thông báo.
+ Kỳ vọng của doanh nghiệp: 
Tự động hóa việc tìm và phân công tài xế.
Quản lý tập trung khách hàng, tài xế, chuyến đi và thanh toán.
Hệ thống ổn định, bảo mật và có khả năng mở rộng.
Có báo cáo, thống kê để quản lý doanh thu và hiệu quả hoạt động.
Dễ dàng bổ sung tính năng và tích hợp dịch vụ mới.
+ Kỳ vọng của khách hàng
Đặt xe nhanh chóng, dễ sử dụng.
Biết được trạng thái chuyến và thông tin tài xế.
Có thể theo dõi chuyến đi.
Thanh toán thuận tiện và an toàn.
Xem lịch sử chuyến, cước phí và đánh giá tài xế.
   
2. Xác định các bên liên quan:
Bên liên quan                                       Vai trò         
+ Khách hàng                               Sử dụng hệ thống để đặt xe, theo dõi chuyến, thanh toán và đánh giá
+ Tài xế                                   Nhận và thực hiện chuyến, cập nhật trạng thái, vị trí và thông tin phương tiện
+ Nhân viên vận hành                       Quản lý khách hàng, tài xế, phương tiện và hỗ trợ xử lý các chuyến có vấn đề
+ Ban giám đốc / Chủ doanh nghiệp          Đưa ra mục tiêu kinh doanh, theo dõi doanh thu, hiệu quả và báo cáo
+ Bộ phận kế toán / tài chính              Theo dõi doanh thu, giao dịch và đối soát thanh toán
+ Bộ phận chăm sóc khách hàng              Tiếp nhận và xử lý khiếu nại, hỗ trợ khách hàng và tài xế
+ Bộ phận kỹ thuật / IT                    Phát triển, triển khai, bảo trì và đảm bảo hệ thống hoạt động ổn định
+ Nhà cung cấp dịch vụ thanh toán          Xử lý các giao dịch thanh toán điện tử bên ngoài CAB
+ Nhà cung cấp dịch vụ bản đồ/GPS          Cung cấp vị trí, bản đồ, khoảng cách và hỗ trợ xác định tài xế gần khách
+ Nhà cung cấp dịch vụ thông báo           Gửi thông báo qua các kênh như SMS, email, push notification,...
+ 
- Xác định tầm quan trọng của Stakeholder:

                         CAB SYSTEM
                             │
          ┌──────────────────┼──────────────────┐
          │                  │                  │
          ▼                  ▼                  ▼
     NGƯỜI DÙNG        QUẢN LÝ NỘI BỘ      BÊN HỖ TRỢ
          │                  │                  │
     ┌────┼────┐        ┌────┼────┐       ┌────┼────┬────┐
     │    │    │        │    │    │       │    │    │    │
    KH   TX    NV      BGĐ  KT   CSKH     IT Thanh toán GPS Thông báo

3. Mục đích nghiệp vụ 
  1. Mục đích nghiệp vụ là gì?

Xây dựng hệ thống thanh toán linh hoạt, cho phép khách hàng thanh toán chi phí chuyến đi bằng tiền mặt hoặc chuyển khoản, tùy theo nhu cầu.

2. Vì sao cần thanh toán tiền mặt?

Đáp ứng những khách hàng có nhu cầu thanh toán trực tiếp cho tài xế và không sử dụng phương thức thanh toán điện tử.

3. Vì sao cần thanh toán chuyển khoản?

Tạo sự thuận tiện cho khách hàng, giúp thanh toán nhanh chóng, không cần sử dụng tiền mặt và dễ dàng ghi nhận giao dịch.

4. Khách hàng được lợi ích gì?

Khách hàng có nhiều lựa chọn thanh toán, thuận tiện và chủ động hơn sau khi hoàn thành chuyến đi.

5. Doanh nghiệp được lợi ích gì?

Doanh nghiệp có thể quản lý và tra cứu giao dịch tập trung, theo dõi doanh thu và hỗ trợ đối soát thanh toán.

6. Nếu chuyển khoản thất bại thì sao?

Hệ thống thông báo cho khách hàng biết giao dịch thất bại và cho phép khách hàng thực hiện thanh toán lại theo chính sách của doanh nghiệp.
| STT | Module                           | Chức năng chính                                                      |
| --- | -------------------------------- | -------------------------------------------------------------------- |
| 1   | **Quản lý tài khoản & xác thực** | Đăng ký, đăng nhập, cập nhật thông tin, phân quyền                   |
| 2   | **Quản lý khách hàng**           | Hồ sơ khách hàng, lịch sử chuyến, đánh giá                           |
| 3   | **Quản lý tài xế**               | Hồ sơ, trạng thái hoạt động, vị trí, thông tin phương tiện           |
| 4   | **Đặt xe (Booking)**             | Điểm đón, điểm đến, loại xe, tạo/hủy yêu cầu                         |
| 5   | **Tìm & phân công tài xế**       | Tìm tài xế phù hợp, ưu tiên tài xế gần, xử lý từ chối/không phản hồi |
| 6   | **Quản lý chuyến đi (Trip)**     | Theo dõi và cập nhật trạng thái chuyến                               |
| 7   | **Bản đồ & GPS**                 | Vị trí tài xế, khoảng cách, hỗ trợ tìm tài xế gần khách              |
| 8   | **Tính cước & thanh toán**       | Tính giá, tiền mặt, chuyển khoản/thanh toán điện tử, xử lý giao dịch |
| 9   | **Thông báo**                    | Thông báo cho khách hàng và tài xế về chuyến đi, thanh toán          |
| 10  | **Đánh giá**                     | Khách hàng đánh giá tài xế sau chuyến                                |
| 11  | **Quản trị vận hành**            | Quản lý khách hàng, tài xế, xe, chuyến và xử lý sự cố                |
| 12  | **Báo cáo & thống kê**           | Chuyến đi, doanh thu, tỷ lệ hoàn thành/hủy, hiệu quả tài xế          |
| 13  | **Audit Log & bảo mật**          | Ghi nhận thao tác quan trọng, kiểm soát quyền truy cập               |



