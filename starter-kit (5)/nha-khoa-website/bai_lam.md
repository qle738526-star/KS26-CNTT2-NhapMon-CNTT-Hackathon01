# BÀI LÀM – HACKATHON 01

- **Mã đề:** 14
- **Họ tên:*Lê Quốc Minh Quân* 
- **Lớp:**CNTT 2 
- **Link repository:** 
- **Hệ điều hành (Windows/macOS):** Window

## 4.2. Thao tác máy tính cơ bản bằng CLI

### Các lệnh đã chạy

```shell
# Ghi lần lượt các lệnh đã chạy, mỗi lệnh một dòng
* Hiển thị đường dẫn tuyệt đối: Get-location.
* Liệt kê tất cả nội dung, bao gồm file ẩn:Get-chiditem. 
* Di chuyển các file: Move-Item -path "huong_dan_cham_soc.txt" -Denstiation "docs\\" và Move-Item -path "logo_nha_khoa.PNG" -Denstiation "media\\".
* Sao chép logo từ media vào backup: cp -path "media\\logo_nha_khoa.PNG" -Denstiation "Backup"
* xóa file .tmp tại thư mục gốc;  không xóa file khác: remove-item -path "nha-khoa-website".
* Đường dẫn tương đối: cd logs ; get-chiditem -path; cd.. 

```

### Kết quả liệt kê toàn bộ dự án (Windows: Get-ChildItem -Recurse -Force; macOS: ls -aR)

```text
 Directory: C:\Users\Quan\Downloads\starter-kit (5)


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----        10/28/2026   1:43 PM                nha-khoa-website


    Directory: C:\Users\Quan\Downloads\starter-kit (5)\nha-khoa-website


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----        10/28/2026   1:48 PM                Nha Khoa Website FINAL
------        10/27/2026   1:32 AM           2224 bai_lam.md


    Directory: C:\Users\Quan\Downloads\starter-kit (5)\nha-khoa-website\Nha Khoa Website FINAL


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
------        10/27/2026   1:32 AM             65 .env
-a----        10/27/2026   1:32 AM           1079 clinic.log.log
-a----        10/27/2026   1:32 AM           6094 dieu_tri_thang_4.xlsx.xlsx
-a----        10/27/2026   1:32 AM             63 huong_dan_cham_soc.txt.txt
-a----        10/27/2026   1:32 AM           5736 logo_nha_khoa.PNG.PNG
------        10/27/2026   1:32 AM             22 temp_226.tmp

```

## 4.3. Lọc log thủ công

### Lệnh đã chạy

```shell
# Ghi lệnh vào đây (xoá dòng này)

```

### 2 dòng lỗi đầu tiên trong daily_report.txt

```text
Get-content logs/clinic.log | select-string "ERROR" > logs/daily_report.txt

```

## 4.4. Thao tác với tài liệu Markdown (README.md)

> README.md được chấm trực tiếp trên file `README.md` ở gốc dự án. Đánh dấu `[x]` vào các mục đã làm để tự kiểm tra.

- [ ] Heading 1: tên dự án
- [ ] Mô tả ngắn có cả **in đậm** và *in nghiêng*
- [ ] Bảng `Thư mục | Nội dung`, ít nhất 3 dòng dữ liệu
- [ ] Code block chứa lệnh PowerShell/Terminal liệt kê nội dung dự án
- [ ] Task list ít nhất 2 công việc, có ít nhất 1 mục đã hoàn thành
- [ ] Blockquote nhắc không upload `.env`

## 4.5. Chạy script auto_report (.ps1 hoặc .sh)

### Lệnh chạy (Windows: nếu dùng Phụ lục 2 thì ghi cả 2 lệnh)

```shell
# Ghi lệnh vào đây (xoá dòng này)

```

### Kết quả hiển thị

```text
(Dán kết quả vào đây – xoá dòng này)

```

## 4.6. Đếm số dòng lỗi

### Lệnh

```shell
# (Get-Content bai_lam.md | Select-String "ERROR").count

```

### Kết quả đếm (Windows: giá trị Count; macOS: con số in ra)

```text
(Dán kết quả vào đây – xoá dòng này)

```

## 4.7. Báo cáo tổng hợp

### Các lệnh đã chạy

```shell
# ===TONG HOP LOG===
(Get-Content clinic.log.log | Select-String "ERROR").Count 
Get-Content clinic.log.log | Select-String "WARNING"

  

```

### Nội dung file logs/tong_hop.txt

```text
PS C:\Users\Quan\Downloads\starter-kit (5)> (Get-Content clinic.log.log | Select-String "ERROR").Count
0

```

## 4.8. Excel

> Phần Excel được chấm trực tiếp trên file `data/dieu_tri_thang_4.xlsx`, không cần ghi vào đây.
u_tri_thang_4.xlsx`, không cần ghi vào đây.
