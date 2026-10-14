# YÊU CẦU ĐẦU RA

## Phần 1: Phân tích

## SƠ ĐỒ MÔ TẢ LUỒNG DỮ LIỆU KHI QUA PIPELINE POWERSHELL

Input:

- Đọc thông tin trong tệp log

Process:

- Lọc và tìm kiếm từ khóa “TIMEOUT” trong tệp
 
- Đếm số lần xuất hiện từ khóa

Output:
- Cho ra kết quả là 1 con số

## Phần 2: Triển khai

-Câu lệnh powershell:
 
 select-string “TIMEOUT” .log| where-object { $_ -notmatch "NOT TIMEOUT" }|measure-object

