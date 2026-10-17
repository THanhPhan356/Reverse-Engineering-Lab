# Reverse Engineering Lab

Repo cá nhân để luyện phân tích binary, khôi phục logic và viết lại chức năng bằng C/C++ hoặc Rust.

## Bắt đầu

Nguồn bài tập: [pwn.college — Reverse Engineering](https://pwn.college/program-security/reverse-engineering/).
Bắt đầu với **Terrible Token (Easy)**, sau đó tăng dần độ khó.

1. Tạo thư mục bài tập, ví dụ `exercises/001-terrible-token/`.
2. Sao chép [mẫu ghi chép](exercise-template.md) thành `README.md` trong thư mục đó.
3. Ghi lại quan sát, giả thuyết và bằng chứng trước khi đọc lời giải.
4. Lưu code tái triển khai và dữ liệu kiểm chứng cạnh ghi chép của bài.

## Cấu trúc mỗi bài

```text
exercises/001-ten-bai/
├── README.md        # Phân tích và kết quả
├── src/             # Code tự viết để tái triển khai hoặc hỗ trợ phân tích
├── tests/           # Dữ liệu và cách đối chiếu hành vi
└── artifacts/       # Binary và dữ liệu cục bộ, không đưa vào Git
```

Chỉ tạo các thư mục con khi cần dùng.

## Tiêu chí hoàn thành

- Giải thích được đầu vào, đầu ra và luồng xử lý chính.
- Phân biệt điều đã xác nhận với giả thuyết còn thiếu bằng chứng.
- Kiểm chứng kết luận bằng debugger, dữ liệu thử hoặc bản tái triển khai.
- Nếu tối ưu: đo độ đúng trước, đo tốc độ sau và ghi điều kiện benchmark.

Binary của bài tập được lưu cục bộ trong `artifacts/`; repo lưu ghi chép và code tự viết.
