Bước 1 — Câu 1: Tìm hiểu nghiệp vụ

a) Hệ thống hiện tại có những vấn đề gì?
- Việc phân công tài xế còn thủ công nên chậm và khó mở rộng.
- Khách hàng khó theo dõi trạng thái chuyến đi, tài xế nhận chuyến và thời gian đón.
- Dữ liệu thanh toán chưa quản lý tập trung, gây khó tra cứu và đối soát.
- Nhân viên vận hành khó theo dõi chuyến đang diễn ra, tình trạng tài xế và xử lý sự cố.
- Hệ thống hiện tại không linh hoạt khi cần thêm tính năng, phương thức thanh toán hoặc kênh thông báo.
  
b) Mục tiêu chính của hệ thống
Xây dựng nền tảng CAB System tự động hóa quy trình đặt xe: khách đặt xe, hệ thống tìm tài xế phù hợp, tài xế nhận chuyến, thực hiện chuyến, tính cước, thanh toán, thông báo và đánh giá. Hệ thống cũng phải hỗ trợ doanh nghiệp quản lý tập trung và mở rộng về sau.

c) Vấn đề hiện tại là gì?

Vấn đề cốt lõi là doanh nghiệp chưa có hệ thống thống nhất để quản lý toàn bộ vòng đời chuyến đi. Điều này làm giảm trải nghiệm khách hàng, tăng áp lực cho tổng đài/vận hành và gây khó khăn khi số lượng khách hàng, tài xế tăng lên.

d) Ai tham gia và sử dụng hệ thống?

- Khách hàng: đăng ký, đặt xe, theo dõi, thanh toán và đánh giá.
- Tài xế: nhận chuyến, cập nhật vị trí và trạng thái chuyến.
- Nhân viên vận hành: quản lý khách hàng, tài xế, chuyến đi, hỗ trợ sự cố.
- Quản trị viên: phân quyền và kiểm tra hoạt động hệ thống.
- Cổng thanh toán và dịch vụ thông báo: hệ thống bên ngoài tích hợp với CAB System.

```
- Sơ đồ tổng quát: 
                         |
       +-----------------+-----------------+
       |                 |                 |
       v                 v                 v
   KHÁCH HÀNG          TÀI XẾ        NHÂN VIÊN VẬN HÀNH
       |                 |                 |
       v                 v                 v
    Đặt xe          Nhận chuyến       Quản lý hệ thống
    Theo dõi        Thực hiện         Theo dõi chuyến
    Thanh toán      Cập nhật          Xử lý sự cố
    Đánh giá        trạng thái        Tra cứu giao dịch
       |                 |                 |
       +-----------------+-----------------+
                         |
                         v
                  HỆ THỐNG CAB
                         |
             +-----------+-----------+
             |                       |
             v                       v
       Nhà cung cấp             Nhà cung cấp
        thanh toán                thông báo
----

Câu 2: Các bên liên quan

| Stakeholder                 | Vai trò                                              |
| --------------------------- | ---------------------------------------------------- |
| Khách hàng                  | Đặt xe, theo dõi chuyến, thanh toán, đánh giá tài xế |
| Tài xế                      | Nhận chuyến, thực hiện chuyến, cập nhật trạng thái   |
| Nhân viên vận hành          | Quản lý khách hàng, tài xế, phương tiện, chuyến đi   |
| Ban lãnh đạo                | Theo dõi doanh thu, số chuyến và hiệu quả hoạt động  |
| Nhà cung cấp thanh toán     | Xử lý giao dịch thanh toán điện tử                   |
| Nhà cung cấp thông báo      | Hỗ trợ gửi thông báo                                 |
| Bộ phận phát triển hệ thống | Phân tích, xây dựng và mở rộng hệ thống              |


Câu 3: Ma trận các bên liên quan (sơ đồ mindmap)
                    STAKEHOLDER MATRIX
              MỨC ĐỘ QUAN TÂM (INTEREST)
                         CAO
                          │
          ┌───────────────┼──────────────────┐
          │               │                  │
          │  THEO DÕI     │   QUẢN LÝ       │
          │  THƯỜNG XUYÊN │   CHẶT CHẼ       │
          │               │                  │
          │ • Kế toán     │ • Ban giám đốc   │
          │ • Nhà cung    │ • Nhân viên      │
          │   cấp thông   │   vận hành       │
          │   báo         │ • Khách hàng     │
          │               │ • Tài xế         │
          │               │                  │
THẤP ─────┼───────────────┼──────────────────┼──── CAO
QUYỀN LỰC │               │                  │  QUYỀN LỰC
(POWER)   │   GIÁM SÁT    │   DUY TRÌ        │
          │   TỐI THIỂU   │   HÀI LÒNG       │
          │               │                  │
          │ • Nhà cung    │ • Business      │
          │   cấp phụ trợ │   Analyst        │
          │               │ • Nhóm phát triển│
          │               │ • Nhà cung cấp   │
          │               │   thanh toán     │
          └───────────────┼──────────────────┘
                          │
                         THẤP
                 MỨC ĐỘ QUAN TÂM





Câu 4: Phạm vi dự án trong 7 tuần

B4. Xác định phạm vi dự án
1. Mục tiêu của phạm vi

Xác định các chức năng cần phát triển trong thời gian 7 tuần, tập trung vào quy trình cốt lõi của CAB System:

Đặt xe → Tìm tài xế → Thực hiện chuyến → Tính cước → Thanh toán → Đánh giá

2. Phạm vi trong dự án
| Nhóm chức năng          | Nội dung                                                            |
| ----------------------- | ------------------------------------------------------------------- |
| **Quản lý tài khoản**   | Đăng ký, đăng nhập, cập nhật thông tin                              |
| **Quản lý khách hàng**  | Quản lý hồ sơ khách hàng                                            |
| **Quản lý tài xế**      | Hồ sơ, trạng thái hoạt động, vị trí                                 |
| **Quản lý phương tiện** | Thông tin xe, loại xe                                               |
| **Đặt xe**              | Nhập điểm đón, điểm đến, chọn loại xe, gửi yêu cầu                  |
| **Tìm tài xế**          | Tìm tài xế phù hợp, gần khách hàng, đang sẵn sàng                   |
| **Phân công chuyến**    | Gửi yêu cầu, xử lý chấp nhận/từ chối                                |
| **Theo dõi chuyến**     | Theo dõi tài xế và trạng thái chuyến                                |
| **Thực hiện chuyến**    | Đã đến, đã đón khách, đang di chuyển, hoàn thành                    |
| **Tính cước**           | Xác định số tiền khách hàng phải trả                                |
| **Thanh toán**          | Tiền mặt và thanh toán điện tử                                      |
| **Thông báo**           | Thông báo đặt xe, nhận chuyến, đến điểm đón, hoàn thành, thanh toán |
| **Đánh giá**            | Khách hàng đánh giá tài xế sau chuyến                               |
| **Quản lý vận hành**    | Theo dõi chuyến, tài xế, xử lý sự cố                                |
| **Báo cáo**             | Số chuyến, doanh thu, hoàn thành, hủy, hiệu quả tài xế              |
| **Phân quyền**          | Kiểm soát quyền của nhân viên vận hành                              |

3. Những nội dung ngoài phạm vi

Trong 7 tuần, không tự mở rộng sang những chức năng chưa được khách hàng yêu cầu hoặc chưa có yêu cầu cụ thể:

Xây dựng hệ thống thanh toán riêng.
Lưu trực tiếp thông tin thẻ/tài khoản ngân hàng.
Xây dựng hệ thống bản đồ/GPS riêng.
AI dự đoán nhu cầu đặt xe.
Chương trình tích điểm/khuyến mãi.
Quảng cáo trên ứng dụng.
Dịch vụ giao hàng.
Xây dựng thêm các loại dịch vụ CAB chưa được xác định.
Tự quyết định chính sách giá, hủy chuyến hoặc ưu tiên tài xế khi khách hàng chưa xác nhận.
4. Các vấn đề chưa xác định – cần BA làm rõ

Đây là phần rất quan trọng 
| STT | Vấn đề cần xác nhận                      |
| --- | ---------------------------------------- |
| 1   | Công thức tính cước cụ thể               |
| 2   | Tiêu chí ưu tiên tài xế                  |
| 3   | Thời gian tài xế phải phản hồi           |
| 4   | Chính sách hủy chuyến                    |
| 5   | Phí hủy chuyến nếu có                    |
| 6   | Số lần thử lại khi thanh toán thất bại   |
| 7   | Cách xử lý khi mất kết nối mạng          |
| 8   | Thời gian lưu trữ dữ liệu                |
| 9   | Quyền hạn cụ thể của từng loại nhân viên |
| 10  | Các chỉ số cần có trong báo cáo          |

--->Trong 7 tuần, nhóm tập trung xây dựng các chức năng cốt lõi giúp CAB vận hành được toàn bộ quy trình đặt xe từ lúc khách hàng tạo yêu cầu đến khi hoàn thành chuyến, thanh toán và đánh giá. Các chức năng mở rộng chưa được khách hàng yêu cầu hoặc chưa có quy tắc nghiệp vụ rõ ràng sẽ được đưa vào danh sách cần xác nhận hoặc xem xét ở giai đoạn sau.
Câu 5: Chuyển các yêu cầu thành yêu cầu nghiệp vụ

Câu 6: Phân rã các yêu cầu chức năng

CAB SYSTEM
│
├── 1. Quản lý tài khoản
│   ├── 1.1 Đăng ký tài khoản
│   ├── 1.2 Đăng nhập
│   ├── 1.3 Cập nhật thông tin cá nhân
│   └── 1.4 Phân quyền người dùng
│
├── 2. Quản lý đặt xe
│   ├── 2.1 Nhập điểm đón
│   ├── 2.2 Nhập điểm đến
│   ├── 2.3 Lựa chọn loại xe
│   ├── 2.4 Gửi yêu cầu đặt xe
│   ├── 2.5 Tìm kiếm tài xế phù hợp
│   └── 2.6 Phân công tài xế
│
├── 3. Quản lý chuyến đi
│   ├── 3.1 Chấp nhận/Từ chối chuyến
│   ├── 3.2 Cập nhật trạng thái chuyến
│   ├── 3.3 Cập nhật vị trí tài xế
│   ├── 3.4 Theo dõi chuyến đi
│   ├── 3.5 Xem lịch sử chuyến
│   └── 3.6 Xử lý chuyến bị lỗi
│
├── 4. Quản lý thanh toán
│   ├── 4.1 Tính cước chuyến đi
│   ├── 4.2 Thanh toán tiền mặt
│   ├── 4.3 Thanh toán điện tử
│   ├── 4.4 Xử lý thanh toán thất bại
│   └── 4.5 Tra cứu giao dịch
│
└── 5. Quản lý vận hành & dịch vụ
    ├── 5.1 Quản lý khách hàng
    ├── 5.2 Quản lý tài xế
    ├── 5.3 Quản lý phương tiện
    ├── 5.4 Gửi thông báo
    ├── 5.5 Đánh giá tài xế
    └── 5.6 Xem báo cáo
Giải thích các nhóm chức năng
1. Quản lý tài khoản

Phục vụ việc xác thực và quản lý người dùng.

Khách hàng đăng ký, đăng nhập.
Khách hàng cập nhật thông tin.
Tài xế quản lý tài khoản.
Nhân viên được phân quyền theo vai trò.
2. Quản lý đặt xe

Đây là chức năng nghiệp vụ trung tâm.

Khách hàng:

Nhập điểm đón → Nhập điểm đến → Chọn loại xe → Gửi yêu cầu

Sau đó hệ thống:

Tìm tài xế → Kiểm tra vị trí/trạng thái/loại xe → Gửi yêu cầu → Phân công tài xế

Nếu tài xế từ chối:

Tài xế A từ chối → tìm tài xế B → tiếp tục cho đến khi có tài xế hoặc hết tài xế phù hợp.

3. Quản lý chuyến đi

Quản lý toàn bộ trạng thái:

Đang tìm tài xế → Đã có tài xế → Tài xế đã đến → Đã đón khách → Đang di chuyển → Hoàn thành

Đồng thời lưu vị trí tài xế và lịch sử chuyến.

4. Quản lý thanh toán

Sau khi chuyến hoàn thành:

Tính cước → Chọn phương thức thanh toán → Xử lý → Ghi nhận kết quả

Có 2 phương thức:

Tiền mặt.
Thanh toán điện tử qua nhà cung cấp bên ngoài.
5. Quản lý vận hành & dịch vụ

Dành chủ yếu cho nhân viên vận hành và ban giám đốc:

Quản lý khách hàng.
Quản lý tài xế.
Quản lý xe.
Gửi thông báo.
Đánh giá tài xế.
Xem báo cáo.

Câu 7: Vẽ Use Case Diagram


                              USE CASE DIAGRAM – CAB SYSTEM


        KHÁCH HÀNG                                           TÀI XẾ
           O                                                   O
          /|\                                                 /|\
          / \                                                 / \
           |                                                   |
           |                                                   |
           |        ┌─────────────────────────────────┐        |
           |        │          CAB SYSTEM             │        |
           ├───────►│                                 │◄───────┤
           |        │       (Đăng ký tài khoản)       │        |
           ├───────►│       (Đăng nhập)               │◄───────┤
           |        │       (Cập nhật thông tin)      │        |
           |        │                                 │        |
           ├───────►│       (Đặt xe)                  │        |
           |        │          │                      │        |
           |        │          ├─<<include>>─(Nhập điểm đón)
           |        │          ├─<<include>>─(Nhập điểm đến)
           |        │          ├─<<include>>─(Chọn loại xe)
           |        │          └─<<include>>─(Tìm tài xế)
           |        │                                 │        |
           ├───────►│       (Theo dõi chuyến)         │◄───────┤
           ├───────►│       (Xem lịch sử chuyến)      │◄───────┤
           ├───────►│       (Thanh toán)              │        |
           |        │          │                      │        |
           |        │          └─<<include>>─(Tính cước)       │
           └───────►│       (Đánh giá tài xế)         │        |
                    │                                 │        |
                    │       (Quản lý hồ sơ)           │◄───────┤
                    │       (Quản lý phương tiện)     │◄───────┤
                    │       (Cập nhật trạng thái)     │◄───────┤
                    │       (Cập nhật vị trí)         │◄───────┤
                    │       (Nhận chuyến)             │◄───────┤
                    │       (Chấp nhận chuyến)        │◄───────┤
                    │       (Từ chối chuyến)          │◄───────┤
                    │       (Cập nhật trạng thái      │◄───────┤
                    │        chuyến)                  │        │
                    │                                 │        │
                    │       (Gửi thông báo)           │        │
                    └─────────────────────────────────┘        │
                                                               │
                                                               │
       NHÂN VIÊN VẬN HÀNH                                      │
                O                                              │
               /|\                                             │
               / \                                             │
                |                                              
                ├──────────────► (Quản lý khách hàng)
                ├──────────────► (Quản lý tài xế)
                ├──────────────► (Quản lý phương tiện)
                ├──────────────► (Theo dõi chuyến)
                ├──────────────► (Xử lý chuyến lỗi)
                ├──────────────► (Tra cứu giao dịch)
                └──────────────► (Xem báo cáo)


          NHÀ CUNG CẤP THANH TOÁN             NHÀ CUNG CẤP THÔNG BÁO

                     O                                  O
                    /|\                                /|\
                    / \                                / \
                     |                                  |
                     └──────► (Thanh toán điện tử)      └──────► (Gửi thông báo)


Câu 8: Đặc tả Use Case
B8. Đặc tả Use Case
UC01 – Đăng ký tài khoản

| Thành phần          | Nội dung                                                                                                                                      |
| ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- |
| **Mã Use Case**     | UC01                                                                                                                                          |
| **Tên**             | Đăng ký tài khoản                                                                                                                             |
| **Actor**           | Khách hàng                                                                                                                                    |
| **Mục tiêu**        | Tạo tài khoản để sử dụng hệ thống                                                                                                             |
| **Điều kiện trước** | Người dùng chưa có tài khoản                                                                                                                  |
| **Điều kiện sau**   | Tài khoản được tạo thành công                                                                                                                 |
| **Luồng chính**     | 1. Người dùng chọn đăng ký → 2. Nhập thông tin → 3. Hệ thống kiểm tra thông tin → 4. Hệ thống tạo tài khoản → 5. Thông báo đăng ký thành công |
| **Ngoại lệ**        | Thông tin không hợp lệ hoặc tài khoản đã tồn tại → thông báo lỗi                                                                              |
UC02 – Đặt xe

| Thành phần          | Nội dung                                                                                                                      |
| ------------------- | ----------------------------------------------------------------------------------------------------------------------------- |
| **Mã Use Case**     | UC02                                                                                                                          |
| **Tên**             | Đặt xe                                                                                                                        |
| **Actor**           | Khách hàng                                                                                                                    |
| **Mục tiêu**        | Tạo yêu cầu đặt xe                                                                                                            |
| **Điều kiện trước** | Khách hàng đã đăng nhập                                                                                                       |
| **Điều kiện sau**   | Yêu cầu đặt xe được tạo                                                                                                       |
| **Luồng chính**     | 1. Nhập điểm đón → 2. Nhập điểm đến → 3. Chọn loại xe → 4. Xác nhận đặt xe → 5. Hệ thống tạo yêu cầu → 6. Hệ thống tìm tài xế |
| **Ngoại lệ**        | Thông tin điểm đón/điểm đến không hợp lệ hoặc không có tài xế phù hợp

   UC03 – Tìm và phân công tài xế

| Thành phần          | Nội dung                                                                                                                                                                                               |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Mã Use Case**     | UC03                                                                                                                                                                                                   |
| **Tên**             | Tìm và phân công tài xế                                                                                                                                                                                |
| **Actor**           | Hệ thống / Tài xế                                                                                                                                                                                      |
| **Mục tiêu**        | Tìm tài xế phù hợp cho chuyến                                                                                                                                                                          |
| **Điều kiện trước** | Có yêu cầu đặt xe                                                                                                                                                                                      |
| **Điều kiện sau**   | Có tài xế nhận chuyến hoặc thông báo không tìm được                                                                                                                                                    |
| **Luồng chính**     | 1. Hệ thống nhận yêu cầu → 2. Xác định vị trí khách → 3. Tìm tài xế đang sẵn sàng → 4. Kiểm tra loại xe → 5. Xác định tài xế phù hợp → 6. Gửi yêu cầu → 7. Tài xế chấp nhận → 8. Gán tài xế cho chuyến |
| **Ngoại lệ**        | Tài xế từ chối/không phản hồi → hệ thống tìm tài xế khác


 UC04 – Theo dõi chuyến đi

| Thành phần          | Nội dung                                                                                                                                |
| ------------------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| **Mã Use Case**     | UC04                                                                                                                                    |
| **Tên**             | Theo dõi chuyến đi                                                                                                                      |
| **Actor**           | Khách hàng                                                                                                                              |
| **Mục tiêu**        | Theo dõi tài xế và trạng thái chuyến                                                                                                    |
| **Điều kiện trước** | Khách hàng có chuyến đang hoạt động                                                                                                     |
| **Điều kiện sau**   | Khách hàng xem được trạng thái hiện tại                                                                                                 |
| **Luồng chính**     | 1. Khách hàng mở chuyến → 2. Hệ thống hiển thị tài xế → 3. Hiển thị vị trí → 4. Hiển thị trạng thái → 5. Cập nhật thông tin theo chuyến |
| **Ngoại lệ**        | Không nhận được dữ liệu vị trí → thông báo trạng thái kết nối                                                                           |
                      |
UC05 – Cập nhật trạng thái chuyến

| Thành phần          | Nội dung                                                                                         |
| ------------------- | ------------------------------------------------------------------------------------------------ |
| **Mã Use Case**     | UC05                                                                                             |
| **Tên**             | Cập nhật trạng thái chuyến                                                                       |
| **Actor**           | Tài xế                                                                                           |
| **Mục tiêu**        | Cập nhật tiến trình chuyến                                                                       |
| **Điều kiện trước** | Tài xế đã nhận chuyến                                                                            |
| **Điều kiện sau**   | Trạng thái chuyến được cập nhật                                                                  |
| **Luồng chính**     | 1. Tài xế nhận chuyến → 2. Đã đến điểm đón → 3. Đã đón khách → 4. Đang di chuyển → 5. Hoàn thành |
| **Ngoại lệ**        | Không thể cập nhật → hệ thống thông báo lỗi và ghi nhận trạng thái gần nhất                      |

UC06 – Thanh toán

| Thành phần          | Nội dung                                                                                                                                                          |
| ------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Mã Use Case**     | UC06                                                                                                                                                              |
| **Tên**             | Thanh toán                                                                                                                                                        |
| **Actor**           | Khách hàng                                                                                                                                                        |
| **Actor phụ**       | Nhà cung cấp thanh toán                                                                                                                                           |
| **Mục tiêu**        | Thanh toán tiền chuyến                                                                                                                                            |
| **Điều kiện trước** | Chuyến đã hoàn thành và đã có cước                                                                                                                                |
| **Điều kiện sau**   | Giao dịch được ghi nhận                                                                                                                                           |
| **Luồng chính**     | 1. Hệ thống tính cước → 2. Khách chọn phương thức → 3. Thanh toán tiền mặt hoặc điện tử → 4. Hệ thống nhận kết quả → 5. Ghi nhận giao dịch → 6. Thông báo kết quả |
| **Ngoại lệ**        | Thanh toán điện tử thất bại → thông báo khách hàng và cho phép xử lý lại theo chính sách                                                                          |

UC07 – Đánh giá tài xế

| Thành phần          | Nội dung                                                                                                         |
| ------------------- | ---------------------------------------------------------------------------------------------------------------- |
| **Mã Use Case**     | UC07                                                                                                             |
| **Tên**             | Đánh giá tài xế                                                                                                  |
| **Actor**           | Khách hàng                                                                                                       |
| **Mục tiêu**        | Đánh giá chất lượng chuyến đi                                                                                    |
| **Điều kiện trước** | Chuyến đã hoàn thành                                                                                             |
| **Điều kiện sau**   | Đánh giá được lưu                                                                                                |
| **Luồng chính**     | 1. Khách hàng mở lịch sử chuyến → 2. Chọn chuyến → 3. Nhập đánh giá → 4. Gửi đánh giá → 5. Hệ thống lưu đánh giá |
| **Ngoại lệ**        | Chuyến chưa hoàn thành → không cho phép đánh giá                                                                 |


UC08 – Quản lý chuyến đi


| Thành phần          | Nội dung                                                                                                               |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------- |
| **Mã Use Case**     | UC08                                                                                                                   |
| **Tên**             | Quản lý chuyến đi                                                                                                      |
| **Actor**           | Nhân viên vận hành                                                                                                     |
| **Mục tiêu**        | Theo dõi và xử lý các chuyến                                                                                           |
| **Điều kiện trước** | Nhân viên đã đăng nhập và có quyền                                                                                     |
| **Điều kiện sau**   | Thông tin chuyến được cập nhật/xử lý                                                                                   |
| **Luồng chính**     | 1. Nhân viên xem danh sách chuyến → 2. Chọn chuyến → 3. Xem trạng thái → 4. Kiểm tra thông tin → 5. Xử lý khi có sự cố |
| **Ngoại lệ**        | Không có quyền → từ chối truy cập                                                                                      |
          |

Câu 9: Phân tích quy trình nghiệp vụ

B9. Phân tích quy trình nghiệp vụ

Ở bước này, mình chọn quy trình nghiệp vụ đặt xe vì đây là quy trình cốt lõi của CAB System. Có thể phân tích bằng Sequence Diagram để thể hiện sự tương tác giữa các bên.

1. Quy trình tổng quát

Khách hàng đặt xe → Hệ thống tiếp nhận → Tìm tài xế → Tài xế nhận chuyến → Thực hiện chuyến → Hoàn thành → Tính cước → Thanh toán → Đánh giá

2. Sequence Diagram
KHÁCH HÀNG          CAB SYSTEM          HỆ THỐNG TÌM TX          TÀI XẾ
     |                   |                     |                    |
     |--- Đặt xe ------->|                     |                    |
     |                   |--- Gửi yêu cầu ---->|                    |
     |                   |                     |--- Tìm TX phù hợp-|
     |                   |                     |------------------->|
     |                   |                     |                    |
     |                   |                     |<-- Chấp nhận ------|
     |                   |<-- Gán tài xế ------|                    |
     |<-- Thông báo -----|                     |                    |
     |                   |                     |                    |
     |                   |<--------------------|<-- Đã đến ----------|
     |<-- Thông báo -----|                     |                    |
     |                   |<--------------------|<-- Đã đón khách ----|
     |                   |                     |                    |
     |                   |<--------------------|<-- Hoàn thành ------|
     |<-- Thông báo -----|                     |                    |
     |                   |                     |                    |
     |<-- Hiển thị cước -|                     |                    |
     |                   |                     |                    |
     |--- Thanh toán --->|                     |                    |
     |                   |--- Yêu cầu -------->| Nhà cung cấp       |
     |                   |<-- Kết quả ---------| thanh toán          |
     |<-- Kết quả -------|                     |                    |
     |                   |                     |                    |
     |--- Đánh giá ----------------------------------------------->|
3. Trường hợp tài xế từ chối
Khách hàng
    │
    ▼
Đặt xe
    │
    ▼
CAB tìm tài xế
    │
    ▼
Gửi yêu cầu cho tài xế A
    │
    ├─── Tài xế A nhận ─────► Gán chuyến
    │
    └─── Tài xế A từ chối
                 │
                 ▼
          Tìm tài xế B
                 │
          ┌──────┴──────┐
          ▼             ▼
       Nhận          Từ chối
          │             │
          ▼             ▼
      Gán chuyến    Tìm tài xế tiếp
                        │
                        ▼
                 Không còn tài xế
                        │
                        ▼
              Thông báo khách hàng

. Các trạng thái của chuyến

Quy trình nghiệp vụ cần quản lý các trạng thái:

Đang tìm tài xế
→ Đã có tài xế
→ Tài xế đã đến
→ Đã đón khách
→ Đang di chuyển
→ Hoàn thành

Nếu có sự cố:

Đang tìm tài xế → Không tìm được tài xế → Hủy/Đóng yêu cầu

hoặc:

Đang thực hiện → Chuyến bị lỗi → Nhân viên vận hành xử lý

5. Kết quả của quy trình

Sau khi hoàn thành quy trình:

Chuyến đi được lưu vào hệ thống.
Cước phí được xác định.
Thanh toán được ghi nhận.
Khách hàng nhận thông báo.
Tài xế có thông tin chuyến/doanh thu.
Khách hàng có thể đánh giá tài xế.
Dữ liệu được lưu để phục vụ tra cứu và báo cáo.

Câu 10: Phân tích các quy tắc nghiệp vụ
| Mã       | Quy tắc nghiệp vụ     | Điều kiện/Nguyên tắc                                                                                        | Đối tượng liên quan  |
| -------- | --------------------- | ----------------------------------------------------------------------------------------------------------- | -------------------- |
| **BR01** | Xác thực người dùng   | Khách hàng và tài xế phải đăng nhập trước khi sử dụng chức năng yêu cầu tài khoản                           | Khách hàng, Tài xế   |
| **BR02** | Đặt xe                | Khách hàng phải cung cấp điểm đón, điểm đến và loại xe trước khi gửi yêu cầu                                | Khách hàng           |
| **BR03** | Tài xế sẵn sàng       | Chỉ tài xế có trạng thái **sẵn sàng** mới được hệ thống đề xuất nhận chuyến                                 | Tài xế, Hệ thống     |
| **BR04** | Tìm tài xế            | Hệ thống ưu tiên tài xế phù hợp dựa trên vị trí, trạng thái và loại xe                                      | Hệ thống             |
| **BR05** | Tài xế không phản hồi | Nếu tài xế không phản hồi trong thời gian quy định, hệ thống phải tiếp tục tìm tài xế khác                  | Hệ thống             |
| **BR06** | Tài xế từ chối        | Nếu tài xế từ chối chuyến, hệ thống không yêu cầu khách hàng đặt lại mà tiếp tục tìm tài xế khác            | Hệ thống             |
| **BR07** | Không tìm được tài xế | Nếu không còn tài xế phù hợp, hệ thống phải thông báo rõ cho khách hàng                                     | Hệ thống, Khách hàng |
| **BR08** | Cập nhật trạng thái   | Tài xế phải cập nhật trạng thái theo tiến trình: đã đến → đã đón khách → đang di chuyển → hoàn thành        | Tài xế               |
| **BR09** | Tính cước             | Cước phí được xác định sau khi chuyến hoàn thành dựa trên loại dịch vụ và thông tin chuyến đi               | Hệ thống             |
| **BR10** | Thanh toán            | Khách hàng được thanh toán bằng tiền mặt hoặc phương thức điện tử                                           | Khách hàng           |
| **BR11** | Bảo mật thanh toán    | CAB System không được lưu trực tiếp thông tin nhạy cảm của thẻ/tài khoản thanh toán                         | Hệ thống             |
| **BR12** | Thanh toán thất bại   | Khi thanh toán điện tử thất bại, hệ thống phải thông báo và cho phép xử lý lại theo chính sách doanh nghiệp | Khách hàng, Hệ thống |
| **BR13** | Đánh giá tài xế       | Chỉ khách hàng đã hoàn thành chuyến mới được đánh giá tài xế                                                | Khách hàng           |
| **BR14** | Phân quyền            | Nhân viên chỉ được thực hiện các chức năng phù hợp với quyền được cấp                                       | Nhân viên            |
| **BR15** | Lưu vết               | Các thao tác quản trị quan trọng phải được ghi log để phục vụ kiểm tra sự cố                                | Hệ thống             |
| **BR16** | Thông báo             | Hệ thống phải gửi thông báo khi đặt xe, có tài xế, tài xế đến, chuyến hoàn thành và thanh toán có kết quả   | Khách hàng, Tài xế   |
| **BR17** | Quản lý vị trí        | Hệ thống lưu thông tin vị trí tài xế để hỗ trợ tìm tài xế và dự kiến thời gian đến                          | Tài xế, Hệ thống     |
| **BR18** | Quản lý chuyến        | Mỗi yêu cầu đặt xe phải có trạng thái để theo dõi trong suốt vòng đời chuyến                                | Hệ thống             |

Các Business Rule chưa được khách hàng chốt

Đây là phần BA bắt buộc phải làm rõ với khách hàng, vì đề đã nói những nội dung này chưa xác định:

| Mã       | Vấn đề cần xác nhận     | Câu hỏi cần đặt ra                                                                |
| -------- | ----------------------- | --------------------------------------------------------------------------------- |
| **BR19** | Cách tính cước          | Cước tính theo km, thời gian hay kết hợp cả hai?                                  |
| **BR20** | Tiêu chí ưu tiên tài xế | Khoảng cách có phải tiêu chí chính không? Có xét đánh giá tài xế không?           |
| **BR21** | Thời gian phản hồi      | Tài xế có bao nhiêu giây để nhận/từ chối chuyến?                                  |
| **BR22** | Hủy chuyến              | Khách hàng và tài xế được hủy trong những trường hợp nào?                         |
| **BR23** | Phí hủy                 | Có tính phí khi khách hàng/tài xế hủy chuyến không?                               |
| **BR24** | Mất kết nối             | Nếu khách hàng hoặc tài xế mất mạng trong lúc đang đi thì hệ thống xử lý thế nào? |
| **BR25** | Lưu trữ dữ liệu         | Dữ liệu chuyến đi, vị trí và giao dịch được lưu trong bao lâu?                    |


Sơ đồ nghiệp vụ: 
                      CAB SYSTEM
                             │
              ┌──────────────┼──────────────┐
              │              │              │
              ▼              ▼              ▼
         ĐẶT XE          TÌM TÀI XẾ      THANH TOÁN
              │              │              │
       Điểm đón/đến     Tài xế sẵn sàng   Chuyến hoàn thành
       Loại xe          Gần khách hàng    Tính cước
              │              │              │
              │         ┌────┴────┐         │
              │         ▼         ▼         │
              │       Nhận      Từ chối     │
              │         │         │         │
              │         │      Tìm TX khác  │
              │         │         │         │
              │         └────┬────┘         │
              │              │              │
              └──────────────┼──────────────┘
                             ▼
                         HOÀN THÀNH
                             │
                    ┌────────┴────────┐
                    ▼                 ▼
                Tiền mặt       Thanh toán điện tử
                                      │
                              Nhà cung cấp thanh toán


                    
