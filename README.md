# BÀI TẬP VỀ NHÀ – MÔN: AN TOÀN VÀ BẢO MẬT THÔNG TIN
  # Chủ đề: Chữ ký số trong file PDF
  # Giảng viên: Đỗ Duy Cốp
  # Sinh viên thực hiện : Lý Văn Kiên
  # Thời điểm giao: 2025-10-24 11:45
  # Đối tượng áp dụng: Toàn bộ sv lớp học phần 58KTPM
  # Hạn nộp: Sv upload tất cả lên github trước 2025-10-31 23:59:59


## Các bước thực hiện : 
bước 1 : khởi tạo kiểm tra (verify_pdf.py chạy với chua_ky.pdf)
👉 Kết quả: Xác thực thất bại, chương trình không tìm thấy trường /ByteRange hoặc /Contents.
📝 Nhận xét: PDF chưa có chữ ký điện tử, hoặc chưa đúng định dạng chứa chữ ký → cần ký lại file gốc trước khi xác thực.
image

bước 2 : ký file (da_ky.py)
👉 Kết quả: Ký thành công, thêm timestamp, tạo file bai_tap_da_ky.pdf.
📝 Nhận xét: Hệ thống ký số hoạt động đúng. Thông tin ký (tên, số điện thoại, địa điểm, số trang) hiển thị đầy đủ và rõ ràng.
image

Ảnh 3 – Giai đoạn xác thực chữ ký (verify_pdf.py với bai_tap_da_ky.pdf`)
👉 Kết quả: Toàn bộ 8 bước xác thực đều “THÀNH CÔNG”.
📝 Nhận xét: Chữ ký hợp lệ, nội dung không bị chỉnh sửa, chứng chỉ tin cậy, có timestamp. Hệ thống xác thực hoạt động đúng.
image

Ảnh 4 – Nội dung file nhat_ky_xac_thuc.txt sau xác minh
👉 Ghi log chi tiết quá trình xác thực, từng bước đều “HỢP LỆ”.
📝 Nhận xét: Nhật ký rõ ràng, minh chứng được việc kiểm tra toàn diện (PKCS7, hash, signature, chain, OCSP, timestamp).
image

Nhận xét tổng thể
Quy trình ký và xác thực chữ ký điện tử hoạt động đúng, đảm bảo tính toàn vẹn và xác thực của tài liệu PDF. File sau khi ký có đầy đủ thông tin người ký, thời gian ký và dấu thời gian hợp lệ. Kết quả xác thực cho thấy chữ ký hợp lệ, dữ liệu không bị chỉnh sửa, chứng chỉ và chuỗi xác thực tin cậy. Hệ thống ghi log rõ ràng, minh chứng đầy đủ cho quá trình kiểm tra.
