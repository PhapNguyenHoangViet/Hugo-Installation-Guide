# Hướng dẫn cài đặt Hugo

## Cách 1: Cài đặt thủ công bằng file biên dịch sẵn 

### Bước 1: Truy cập trang latest release
- Truy cập trang [latest release](https://github.com/gohugoio/hugo/releases) và cuộn xuống phần **Assets**.

### Bước 2: Tải về file phù hợp
- Tải về file tương ứng với phiên bản và hệ điều hành bạn cần.
- Link tải nhanh cho Windows: [Hugo_v0.140.2](https://github.com/gohugoio/hugo/releases/download/v0.140.2/hugo_extended_0.140.2_Windows-64bit.zip).

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
3. Nếu lệnh trả về phiên bản Hugo, bạn đã cài đặt thành công.


## Cách 2: Cài Đặt Hugo Bằng Package Manager (Chocolatey)

### Bước 1: Mở Windows PowerShell (Admin)
- Nhấn **Windows + S**, tìm **Windows PowerShell**.
- Nhấp chuột phải vào **Windows PowerShell** và chọn **Run as Administrator**.

### Bước 2: Cài Đặt Chocolatey
1. Sao chép và dán lệnh sau vào PowerShell và nhấn **Enter**:
   ```bash
   Get-ExecutionPolicy
   ```
2. Nếu kết quả trả về là Restricted, bạn có thể dán một trong các lệnh sau:
   ```bash
   Set-ExecutionPolicy AllSigned
   ```
   hoặc:
   ```bash
   Set-ExecutionPolicy Bypass -Scope Process
   ```
3. Cài đặt Chocolatey bằng lệnh
   ```bash
   Set-ExecutionPolicy Bypass -Scope Process -Force; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
   ```

### Bước 3: Xác minh cài đặt Chocolatey
1. Sau khi cài đặt hoàn tất, khởi động lại PowerShell.
2. Kiểm tra phiên bản Chocolatey đã cài đặt bằng lệnh:
   ```bash
   choco --version
   ```
3. Nếu lệnh trả về phiên bản của Chocolatey, cài đặt đã thành công.

### Bước 4: Cài đặt Hugo Extended Edition
1. Mở Command Prompt hoặc PowerShell với quyền admin.
2. Chạy lệnh sau để cài đặt Hugo Extended Edition:
   ```bash
   choco install hugo-extended
   ```

### Bước 5: Cài đặt Hugo Extended Edition
1. Mở PowerShell hoặc Command Prompt.
2. Chạy lệnh sau để kiểm tra phiên bản của Hugo:
   ```bash
   hugo version
   ```