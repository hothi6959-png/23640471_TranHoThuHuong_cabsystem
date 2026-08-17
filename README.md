
# 1. Đặt câu hỏi

## 1.1. Vấn đề hiện tại: Tìm tài xế thủ công, không theo dõi được trạng thái chuyến đi

* Hiện tại doanh nghiệp đang phân công tài xế cho khách hàng bằng cách nào?
* Ai là người thực hiện việc phân công tài xế?
* Khi khách hàng đặt xe, khách hàng có biết hệ thống đang tìm tài xế hay không?
* Khách hàng hiện có thể biết tài xế nào đã nhận chuyến không?
* Khách hàng có thể theo dõi trạng thái chuyến đi đến mức nào?
* Khi tài xế không nhận hoặc từ chối chuyến, hiện tại doanh nghiệp xử lý như thế nào?
* Những khó khăn thường gặp khi phân công tài xế là gì?

## 1.2. Tại sao cần hệ thống mới?

* Mục tiêu quan trọng nhất khi xây dựng hệ thống CAB mới là gì?
* Doanh nghiệp muốn cải thiện vấn đề nào trước tiên?
* Hệ thống mới cần phục vụ khoảng bao nhiêu khách hàng và tài xế?
* Những chức năng của hệ thống hiện tại có cần giữ lại không?
* Doanh nghiệp mong muốn hệ thống phát triển thêm những chức năng nào trong tương lai?

## 1.3. Hệ thống mới giúp ích gì?

* Hệ thống cần hỗ trợ những công việc nào cho khách hàng?
* Hệ thống cần hỗ trợ những công việc nào cho tài xế?
* Nhân viên vận hành cần quản lý những thông tin nào?
* Ban lãnh đạo cần những báo cáo nào để theo dõi hoạt động?
* Hệ thống cần giúp doanh nghiệp giảm những công việc thủ công nào?

# 2. Xác định Stakeholder, vai trò và tầm quan trọng

| Stakeholder                 | Vai trò                                              | Mức độ quan trọng |
| --------------------------- | ---------------------------------------------------- | ----------------- |
| Khách hàng                  | Đặt xe, theo dõi chuyến, thanh toán, đánh giá tài xế | Rất cao           |
| Tài xế                      | Nhận chuyến, thực hiện chuyến, cập nhật trạng thái   | Rất cao           |
| Nhân viên vận hành          | Quản lý khách hàng, tài xế, phương tiện và chuyến đi | Rất cao           |
| Ban lãnh đạo                | Theo dõi doanh thu, số chuyến và hiệu quả hoạt động  | Cao               |
| Nhà cung cấp thanh toán     | Xử lý các giao dịch thanh toán điện tử               | Cao               |
| Nhà cung cấp thông báo      | Hỗ trợ gửi thông báo cho khách hàng và tài xế        | Trung bình – Cao  |
| Bộ phận phát triển hệ thống | Phân tích, xây dựng và mở rộng hệ thống              | Cao               |

Tài liệu xác định ba nhóm người dùng chính là **khách hàng, tài xế và nhân viên vận hành**, đồng thời có nhu cầu báo cáo cho ban lãnh đạo.

# 3. Mục đích kinh doanh

## Mục tiêu chính

Xây dựng một nền tảng CAB đặt xe trực tuyến có khả năng phục vụ số lượng lớn khách hàng và tài xế, giảm các thao tác thủ công và tạo nền tảng có thể mở rộng trong tương lai.

## Các mục tiêu cụ thể

* Tự động hóa việc tìm kiếm và phân công tài xế.
* Cho phép khách hàng theo dõi trạng thái chuyến đi.
* Hỗ trợ tính cước và thanh toán.
* Hỗ trợ tài xế quản lý và cập nhật chuyến đi.
* Hỗ trợ nhân viên vận hành quản lý khách hàng, tài xế, phương tiện và chuyến đi.
* Cung cấp báo cáo về số chuyến, doanh thu, tỷ lệ hoàn thành, tỷ lệ hủy và hiệu quả tài xế.
* Bảo vệ thông tin cá nhân, vị trí và dữ liệu giao dịch.
* Xây dựng hệ thống có khả năng mở rộng và bổ sung chức năng trong tương lai.

# 4. Xác định phạm vi dự án

## Trong phạm vi

### Khách hàng

* Đăng ký, đăng nhập.
* Cập nhật thông tin cá nhân.
* Nhập điểm đón và điểm đến.
* Chọn loại xe.
* Đặt xe.
* Theo dõi trạng thái chuyến.
* Xem lịch sử chuyến đi.
* Xem số tiền phải trả.
* Thanh toán.
* Đánh giá tài xế.

### Tài xế

* Đăng ký hoặc được nhân viên tạo tài khoản.
* Cập nhật hồ sơ.
* Quản lý thông tin phương tiện.
* Cập nhật trạng thái hoạt động.
* Nhận thông báo chuyến mới.
* Chấp nhận hoặc từ chối chuyến.
* Cập nhật trạng thái chuyến.
* Cung cấp thông tin vị trí.

### Nhân viên vận hành

* Quản lý khách hàng.
* Quản lý tài xế.
* Quản lý phương tiện.
* Quản lý chuyến đi.
* Theo dõi chuyến đang diễn ra.
* Kiểm tra trạng thái tài xế.
* Xử lý các trường hợp chuyến bị lỗi.
* Tra cứu lịch sử giao dịch.

### Báo cáo

* Số lượng chuyến.
* Doanh thu.
* Tỷ lệ chuyến hoàn thành.
* Tỷ lệ hủy.
* Hiệu quả hoạt động của tài xế.

## Ngoài phạm vi/chưa xác định

Các nội dung sau **chưa được doanh nghiệp chốt** và cần phỏng vấn thêm:

* Công thức tính cước cụ thể.
* Tiêu chí ưu tiên tài xế.
* Thời gian tài xế phải phản hồi.
* Chính sách hủy chuyến.
* Cách xử lý khi mất kết nối mạng.
* Thời gian lưu trữ dữ liệu.

# 5. Yêu cầu nghiệp vụ (Business Requirements)

**BR01:** Xây dựng nền tảng CAB đặt xe trực tuyến.

**BR02:** Tự động hóa việc tìm và phân công tài xế.

**BR03:** Cho phép khách hàng đặt xe và theo dõi chuyến đi.

**BR04:** Hỗ trợ tài xế tiếp nhận và thực hiện chuyến.

**BR05:** Hỗ trợ tính cước và thanh toán.

**BR06:** Hỗ trợ quản lý khách hàng, tài xế, phương tiện và chuyến đi.

**BR07:** Cung cấp thông báo cho khách hàng và tài xế.

**BR08:** Cung cấp báo cáo phục vụ quản lý và ra quyết định.

**BR09:** Đảm bảo hệ thống hoạt động ổn định khi nhu cầu tăng cao.

**BR10:** Xây dựng hệ thống có khả năng mở rộng để bổ sung dịch vụ, phương thức thanh toán và nhà cung cấp thông báo trong tương lai.

# 6. Quy trình nghiệp vụ

**Quy trình đặt xe:**

Khách hàng
→ Đăng nhập
→ Nhập điểm đón/điểm đến
→ Chọn loại xe
→ Gửi yêu cầu đặt xe
→ Hệ thống tìm tài xế phù hợp
→ Gửi yêu cầu cho tài xế
→ Tài xế chấp nhận/từ chối
→ Nếu từ chối hoặc không phản hồi → tìm tài xế khác
→ Nếu có tài xế → thông báo cho khách hàng
→ Tài xế đến điểm đón
→ Đón khách
→ Thực hiện chuyến
→ Hoàn thành chuyến
→ Hệ thống tính cước
→ Khách hàng thanh toán
→ Hệ thống thông báo kết quả
→ Khách hàng đánh giá tài xế.

Nếu không tìm được tài xế, hệ thống phải thông báo rõ cho khách hàng.

# 7. Yêu cầu chức năng

| Mã   | Yêu cầu chức năng                                                            |
| ---- | ---------------------------------------------------------------------------- |
| FR01 | Hệ thống cho phép khách hàng đăng ký tài khoản.                              |
| FR02 | Hệ thống cho phép người dùng đăng nhập và xác thực.                          |
| FR03 | Hệ thống cho phép khách hàng cập nhật thông tin cá nhân.                     |
| FR04 | Hệ thống cho phép khách hàng nhập điểm đón, điểm đến và chọn loại xe.        |
| FR05 | Hệ thống tiếp nhận yêu cầu đặt xe.                                           |
| FR06 | Hệ thống tìm tài xế phù hợp dựa trên vị trí và trạng thái sẵn sàng.          |
| FR07 | Hệ thống gửi yêu cầu chuyến đến tài xế phù hợp.                              |
| FR08 | Tài xế có thể chấp nhận hoặc từ chối chuyến.                                 |
| FR09 | Hệ thống tiếp tục tìm tài xế khác nếu tài xế được đề xuất không nhận chuyến. |
| FR10 | Khách hàng theo dõi được trạng thái chuyến đi.                               |
| FR11 | Tài xế cập nhật trạng thái chuyến.                                           |
| FR12 | Hệ thống lưu thông tin vị trí của tài xế.                                    |
| FR13 | Hệ thống tính số tiền khách hàng phải trả.                                   |
| FR14 | Hệ thống hỗ trợ thanh toán tiền mặt và thanh toán điện tử.                   |
| FR15 | Hệ thống kết nối với nhà cung cấp thanh toán bên ngoài.                      |
| FR16 | Hệ thống gửi thông báo cho khách hàng và tài xế.                             |
| FR17 | Nhân viên vận hành quản lý khách hàng, tài xế, phương tiện và chuyến đi.     |
| FR18 | Nhân viên vận hành theo dõi các chuyến đang diễn ra.                         |
| FR19 | Nhân viên tra cứu lịch sử giao dịch.                                         |
| FR20 | Hệ thống hỗ trợ phân quyền thao tác quản trị.                                |
| FR21 | Hệ thống cung cấp báo cáo hoạt động.                                         |
| FR22 | Khách hàng có thể đánh giá tài xế sau chuyến đi.                             |

Các chức năng trên được tổng hợp trực tiếp từ nhu cầu của khách hàng trong tài liệu.

# 8. Yêu cầu phi chức năng

| Mã    | Yêu cầu phi chức năng                                                                                        |
| ----- | ------------------------------------------------------------------------------------------------------------ |
| NFR01 | Hệ thống phải hoạt động ổn định khi số lượng người dùng tăng cao.                                            |
| NFR02 | Các thành phần của hệ thống có khả năng mở rộng độc lập khi tải tăng.                                        |
| NFR03 | Lỗi ở thanh toán hoặc thông báo không được làm toàn bộ hệ thống đặt xe ngừng hoạt động.                      |
| NFR04 | Chức năng mới có thể triển khai từng phần và hạn chế ảnh hưởng đến chức năng đang hoạt động.                 |
| NFR05 | Người dùng phải được xác thực trước khi sử dụng chức năng yêu cầu tài khoản.                                 |
| NFR06 | Chức năng quản trị phải được kiểm soát quyền truy cập.                                                       |
| NFR07 | Thông tin cá nhân, phương tiện, vị trí và giao dịch phải được bảo vệ.                                        |
| NFR08 | Hệ thống phải lưu vết các thao tác quan trọng để phục vụ kiểm tra khi có sự cố.                              |
| NFR09 | Kiến trúc phải đủ linh hoạt để bổ sung dịch vụ và phương thức thanh toán mới.                                |
| NFR10 | Có thể thay đổi thành phần kỹ thuật hoặc nhà cung cấp thông báo mà không phải xây dựng lại toàn bộ ứng dụng. |

Các yêu cầu về ổn định, mở rộng, bảo mật và lưu vết được nêu rõ trong tài liệu.

# 9. Quy tắc nghiệp vụ

**BRULE01 – Xác thực:**
Khách hàng và tài xế phải được xác thực trước khi sử dụng các chức năng yêu cầu tài khoản.

**BRULE02 – Phân tài xế:**
Tài xế được lựa chọn dựa trên vị trí, trạng thái sẵn sàng và các tiêu chí vận hành.

**BRULE03 – Tìm tài xế thay thế:**
Nếu tài xế được đề xuất không phản hồi hoặc từ chối chuyến, hệ thống phải tiếp tục tìm tài xế khác.

**BRULE04 – Không có tài xế:**
Nếu không tìm được tài xế, hệ thống phải thông báo rõ cho khách hàng.

**BRULE05 – Thanh toán:**
Khách hàng có thể thanh toán bằng tiền mặt hoặc phương thức thanh toán điện tử.

**BRULE06 – Thông tin thanh toán:**
Thông tin nhạy cảm của thẻ hoặc tài khoản thanh toán không được lưu trực tiếp trong hệ thống CAB.

**BRULE07 – Trạng thái chuyến:**
Tài xế phải cập nhật trạng thái trong quá trình thực hiện chuyến, gồm: đến điểm đón, đã đón khách, đang di chuyển và hoàn thành chuyến.

**BRULE08 – Phân quyền:**
Các thao tác quản trị nhạy cảm chỉ được thực hiện bởi nhân viên có quyền phù hợp.

**BRULE09 – Đánh giá:**
Khách hàng được đánh giá tài xế sau khi chuyến đi hoàn thành.

**BRULE10 – Bảo vệ dữ liệu:**
Thông tin cá nhân, thông tin phương tiện, dữ liệu vị trí và dữ liệu giao dịch phải được bảo vệ.

## Những quy tắc cần xác nhận thêm với khách hàng

* Công thức tính cước.
* Tiêu chí cụ thể để ưu tiên tài xế.
* Thời gian chờ phản hồi của tài xế.
* Chính sách hủy chuyến.
* Xử lý khi mất kết nối mạng.
* Thời gian lưu trữ dữ liệu.

Đây là các điểm **chưa đủ thông tin để BA tự kết luận**, nên cần đưa vào phỏng vấn/xác nhận với stakeholder trước khi nhóm phát triển xây dựng hệ thống.
