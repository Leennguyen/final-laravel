account linh.nguyenthikhanh02@gmail.com
mk: khanhlinh
# Các tạo domain ảo
đầu tiên đăng ký tài khoản google analytics
tiếp theo là tạo tên miền ảo trên xampp cho project
Bước 1: Cấu hình lại file hosts
C:\Windows\System32\drivers\etc
Sau đó bạn truy mở file host bằng phần mềm notepadd++  sau đến cuối file thiết lập trỏ ip về tên miền ảo của mình.
Bước 2: Khai báo tên miền ảo
C:\xampp\apache\conf\extra\
Sau đó mở file httpd-vhosts.conf lên trong trình notepad++. Bạn thêm đoạn code trên vào cuối file.

<VirtualHost *:80>
    DocumentRoot "C:/xampp/htdocs/unitopdev.com"
    ServerName unitopdev.com
</VirtualHost> 
DocumentRoot: Đường dẫn đến thư mục dự án trên xampp
ServerName: Tên miền ảo muốn thiết lập
Ở bước này nếu bạn chọn domain có đuôi .dev thường bị trình duyệt chặn bảo mật, vậy nên bạn cứ đặt .com nhé.
Chạy tên miền ảo
Lỗi: Fatal error: Class 'Illuminate\Foundation\Application' not found in C:\cms\bootstrap\app.php on line 14
