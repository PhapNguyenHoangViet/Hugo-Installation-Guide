# Hướng Dẫn Cài Đặt Hugo

## Cách 1: Cài Đặt Thủ Công Bằng File Biên Dịch Sẵn

### Bước 1: Truy cập trang latest release
- Truy cập trang [latest release](https://github.com/gohugoio/hugo/releases) và cuộn xuống phần **Assets**.

### Bước 2: Tải về file phù hợp
- Tải về file tương ứng với phiên bản và hệ điều hành bạn cần.
- [Link tải nhanh cho Windows: Hugo_v0.140.2](https://github.com/gohugoio/hugo/releases/download/v0.140.2/hugo_extended_0.140.2_Windows-64bit.zip).

### Bước 3: Giải nén và di chuyển tệp
- Giải nén tệp và di chuyển tệp thực thi (file `.exe`) đến thư mục bạn muốn (ví dụ: `C:\Hugo`).

### Bước 4: Thêm thư mục vào biến môi trường PATH
1. Nhấn **Windows + S**, tìm **Environment Variables**.
2. Chọn **Edit the system environment variables**.
3. Trong tab **Advanced**, nhấn **Environment Variables**.
4. Chọn **Path** trong **System variables**, nhấn **Edit**.
5. Nhấn **New**, thêm đường dẫn đến thư mục chứa Hugo (ví dụ: `C:\Hugo`).
6. Nhấn **OK** để lưu.

### Bước 5: Kiểm tra cài đặt
1. Mở **Command Prompt** hoặc **PowerShell**.
2. Chạy lệnh:
   ```bash
   hugo version
   ```