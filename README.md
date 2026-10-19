# Bảng tính lãi tiền gửi

Website tĩnh, gồm `index.html` và thư mục `fonts/` chứa font Lora cùng giấy phép. Không cần cài Node.js, cơ sở dữ liệu hoặc cấu hình biến môi trường.

## Đưa lên GitHub và Tenten

1. Giải nén file ZIP. Giữ `index.html` ở thư mục gốc của repository GitHub (không đặt trong thư mục con).
2. Tạo repository GitHub rồi tải `index.html`, `README.md` và cả thư mục `fonts/` lên.
3. Trong Tenten Vibe Code Hosting, mở **Tenten 1-Click Launch Website** → tạo dự án → chọn nguồn GitHub, dán liên kết repository, chọn tên miền và triển khai. Bạn cũng có thể tải trực tiếp file ZIP lên Tenten.

Ngày gửi trên trang lấy theo múi giờ `Asia/Ho_Chi_Minh` (UTC+7). Trang ước tính theo lãi suất đầu vào 8,7%/năm. Các kỳ hạn hiện có là 6, 11, 12 và 13 tháng; ngày tất toán được tính bằng cách cộng đúng số tháng theo lịch. Lãi được làm tròn đến đồng theo từng kỳ.

Sổ tiếp theo được đưa vào phép tính khi lãi của sổ liền trước đạt từ 1.000.000 đồng; nếu thấp hơn mức này thì dừng. Bảng chi tiết thay phần thẻ cũ: mỗi dòng thể hiện nguồn vốn, vốn tính lãi, số ngày, lãi suất, công thức `vốn × 8,70% × số ngày / 365` và tiền lãi đã làm tròn đến đồng. Phần đầu bảng cho biết ngày gửi và ngày tất toán của kỳ hạn đang chọn. Ảnh chụp bảng tính cũng hiển thị công thức từng sổ. Ô **Số tiền chi thêm** mặc định bằng 0; khoản này và tiền thưởng theo quy tắc hiện tại được cộng vào vốn tái gửi của Sổ 2 cùng với lãi Sổ 1. Từ Sổ 3 trở đi, vốn mỗi sổ tiếp tục lấy từ tiền lãi sổ liền trước. Mức thưởng vẫn tính theo quy tắc cũ dựa trên số tiền gửi và kỳ hạn đã chọn; khoản thưởng được hiển thị riêng, không cộng lặp lại vào kết quả cuối kỳ. Đây là mô phỏng theo các thông số đầu vào, không bảo đảm lãi suất hay việc được nhận quà; khách hàng cần đối chiếu thể lệ, điều kiện và lãi suất trực tiếp với tổ chức cung cấp.

Quà tặng theo bảng: kỳ hạn 6 và 11 tháng nhận lần lượt 1 triệu, 4 triệu, 10 triệu, 30 triệu, 60 triệu và 150 triệu theo các mốc từ 500 triệu đến dưới 2 tỷ, từ 2 tỷ đến dưới 5 tỷ, từ 5 tỷ đến dưới 10 tỷ, từ 10 tỷ đến dưới 20 tỷ, từ 20 tỷ đến dưới 50 tỷ và từ 50 tỷ trở lên. Kỳ hạn 12 và 13 tháng nhận lần lượt 500 nghìn, 2 triệu, 5 triệu, 20 triệu, 40 triệu và 100 triệu theo cùng các mốc tiền gửi. Dưới 500 triệu không có quà tặng.

Trang hiển thị thương hiệu **Chi nhánh Thăng Long**. Bố cục xếp thông tin nhập và kết quả thành các phần toàn chiều rộng; bảng công thức giữ đủ cột trên màn hình lớn và chuyển thành từng thẻ thông tin trên điện thoại, không cần kéo ngang. Khối thu thập số điện thoại và tích hợp EmailJS đã được gỡ bỏ theo yêu cầu.

Các phương án chia sổ được trình bày theo nhóm dễ đọc: các sổ có cùng số tiền và kỳ hạn sẽ được gom lại, ví dụ `3 sổ × 2 tỷ · 6 tháng + 600 triệu · 6 tháng`, nhưng số liệu tính toán gốc vẫn giữ nguyên.

Khu vực **Chụp và chia sẻ kết quả** có ba lựa chọn: chụp riêng mục bảng tính thông thường, chụp riêng các phương án tham khảo hoặc chụp tổng thể cả hai phần. Nút **Chia sẻ ảnh đã tạo** mở bảng chia sẻ của thiết bị; nếu trình duyệt không hỗ trợ chia sẻ tệp nhưng cho phép sao chép ảnh, ảnh sẽ được sao chép để dán vào ứng dụng nhắn tin.

Trang cũng có phần **Phương án tham khảo theo số tiền đang nhập**. Phần này lấy số tiền và kỳ hạn khách chọn làm phương án chính, trình bày cách phân bổ sổ và cho xem các kỳ hạn dài hơn đang có. Mỗi phương án hiển thị cách chia, tiền lãi, quà tham khảo, tổng lợi ích, số tiền cuối kỳ và **Lãi suất thực nhận + Quà quy đổi** theo năm để so sánh các kỳ hạn.
