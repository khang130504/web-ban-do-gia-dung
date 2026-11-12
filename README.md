# Gia Dụng Shop

Website bán đồ gia dụng bằng PHP 8.2 và MySQL/MariaDB, chạy trên XAMPP. Có quản trị, tài khoản, danh mục, biến thể sản phẩm, giỏ hàng, voucher, chatbot, Google/Facebook OAuth và VNPAY sandbox.

## Chạy trên XAMPP

1. Bật Apache và MySQL trên XAMPP có PHP 8.2 trở lên.
2. Đặt mã nguồn trong `XAMPP/htdocs/web-ban-do-gia-dung`.
3. Từ thư mục dự án, chạy `php scripts/setup.php` bằng PHP của XAMPP. Script nhập dữ liệu mẫu khi cơ sở dữ liệu trống và áp dụng các migration.
4. Mở <http://localhost/web-ban-do-gia-dung/>.

Tài khoản mẫu `admin` và `user` dùng mật khẩu `password`. Chỉ dùng các tài khoản mẫu trên localhost.

## Cấu hình dịch vụ

Dùng `config/local.example.php` làm mẫu cho `config/local.php`. Google OAuth dùng callback localhost. Facebook OAuth và VNPAY IPN cần callback HTTPS. Lưu khóa dịch vụ và bản sao lưu cơ sở dữ liệu bên ngoài Git.
