# BÀI TẬP VỀ NHÀ – MÔN: AN TOÀN VÀ BẢO MẬT THÔNG TIN
  # Chủ đề: Chữ ký số trong file PDF
  # Giảng viên: Đỗ Duy Cốp
  # Sinh viên thực hiện : Lý Văn Kiên
  # Thời điểm giao: 2025-10-24 11:45
  # Đối tượng áp dụng: Toàn bộ sv lớp học phần 58KTPM
  # Hạn nộp:  2025-10-31 23:59:59


## Các bước thực hiện : 
bước 1 : khởi tạo kiểm tra (verify_pdf.py chạy với khoidau.pdf)
 Kết quả: Xác thực thất bại, chương trình không tìm thấy trường /ByteRange hoặc /Contents.
 Nhận xét: PDF chưa có chữ ký điện tử, hoặc chưa đúng định dạng chứa chữ ký → cần ký lại file gốc trước khi xác thực.
image

bước 2 : ký file (daky.py)
 Kết quả: Ký thành công, thêm timestamp, tạo file chudaky.pdf.
 Nhận xét: Hệ thống ký số hoạt động đúng. Thông tin ký (tên, số điện thoại, địa điểm, số trang) hiển thị đầy đủ và rõ ràng.
image

bước 3 : xác thực chữ ký (verify_pdf.py với chudaky.pdf`)
 Kết quả: Toàn bộ 8 bước xác thực đều “THÀNH CÔNG”.
 Nhận xét: Chữ ký hợp lệ, nội dung không bị chỉnh sửa, chứng chỉ tin cậy, có timestamp. Hệ thống xác thực hoạt động đúng.
image


