# Bảng tính lãi tiền gửi

Website tĩnh, gồm `index.html` và thư mục `fonts/` chứa font Lora cùng giấy phép. Không cần cài Node.js, cơ sở dữ liệu hoặc cấu hình biến môi trường.

## Đưa lên GitHub và Tenten

1. Giải nén file ZIP. Giữ `index.html` ở thư mục gốc của repository GitHub (không đặt trong thư mục con).
2. Tạo repository GitHub rồi tải `index.html`, `README.md` và cả thư mục `fonts/` lên.
3. Trong Tenten Vibe Code Hosting, mở **Tenten 1-Click Launch Website** → tạo dự án → chọn nguồn GitHub, dán liên kết repository, chọn tên miền và triển khai. Bạn cũng có thể tải trực tiếp file ZIP lên Tenten.

Ngày gửi trên trang lấy theo múi giờ `Asia/Ho_Chi_Minh` (UTC+7). Trang tính ngày tất toán theo kỳ hạn và dùng lãi suất 8,8%/năm. Các kỳ hạn hiện có là 6, 11, 12 và 13 tháng; ngày tất toán được tính bằng cách cộng đúng số tháng theo lịch.

Quà tặng theo bảng: kỳ hạn 6 và 11 tháng nhận lần lượt 1 triệu, 4 triệu, 10 triệu, 30 triệu, 60 triệu và 150 triệu theo các mốc từ 500 triệu đến dưới 2 tỷ, từ 2 tỷ đến dưới 5 tỷ, từ 5 tỷ đến dưới 10 tỷ, từ 10 tỷ đến dưới 20 tỷ, từ 20 tỷ đến dưới 50 tỷ và từ 50 tỷ trở lên. Kỳ hạn 12 và 13 tháng nhận lần lượt 500 nghìn, 2 triệu, 5 triệu, 20 triệu, 40 triệu và 100 triệu theo cùng các mốc tiền gửi. Dưới 500 triệu không có quà tặng.

Trang có thương hiệu **Thăng Long** ở phần đầu trang và hệ thống tiêu đề được phân cấp bằng màu xanh đậm cùng điểm nhấn vàng, ưu tiên dễ đọc trên máy tính và điện thoại.

Khu vực **Chụp và chia sẻ kết quả** có ba lựa chọn: chụp riêng mục bảng tính thông thường, chụp riêng các phương án tối ưu hoặc chụp tổng thể cả hai phần. Nút **Chia sẻ ảnh đã tạo** mở bảng chia sẻ của thiết bị; nếu trình duyệt không hỗ trợ chia sẻ tệp nhưng cho phép sao chép ảnh, ảnh sẽ được sao chép để dán vào ứng dụng nhắn tin.

Trang cũng có phần **Phương án theo yêu cầu khách hàng**. Phần này lấy đúng số tiền và kỳ hạn khách chọn làm phương án chính, tự chia sổ tối ưu trong kỳ hạn đó, rồi chỉ hiển thị các kỳ hạn dài hơn để đề xuất thêm. Mỗi phương án hiển thị số tiền chia, tiền lãi, quà tặng, tổng lợi ích, số tiền cuối kỳ và **Lãi suất thực nhận + Quà quy đổi** theo năm để so sánh các kỳ hạn.
