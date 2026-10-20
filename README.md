# DoAnWEB
Website bán quần áo
2. KHỞI CHẠY WEBSITE TRÊN XAMPP

Yêu cầu: máy tính Windows có XAMPP (Apache và MySQL/MariaDB), trình duyệt web và thư mục dự án FashionStore được giải nén đầy đủ.

2.1. Cài đặt lần đầu trên máy mới

1. Giải nén thư mục dự án sao cho thư mục gốc ban-quan-ao nằm trong thư mục htdocs của XAMPP. Ví dụ: C:\xampp\htdocs\ban-quan-ao. Nếu cài XAMPP ở ổ D:, hãy dùng đúng đường dẫn cài đặt trên máy.

2. Mở XAMPP Control Panel và nhấn Start ở hai dịch vụ Apache và MySQL. Cả hai dịch vụ cần đang chạy để website hoạt động.

3. Mở http://localhost/phpmyadmin. Chọn chức năng Import và nhập file db.sql có trong thư mục dự án để tạo cơ sở dữ liệu shop_quan_ao cùng dữ liệu mẫu.

4. Nhập tiếp file update_images.sql nếu cần gán đường dẫn ảnh sản phẩm mẫu với các ảnh có sẵn trong thư mục assets/images/products.

5. Tạo tài khoản quản trị bằng cách mở http://localhost/ban-quan-ao/admin/setup_admin.php một lần. Tài khoản mẫu được thiết lập là admin@fashionstore.local, mật khẩu admin123.

6. Sau khi thiết lập Admin thành công, nên xóa hoặc đổi tên file admin/setup_admin.php trên bản chạy để tránh người khác gọi lại trang thiết lập tài khoản.

7. Mở http://localhost/ban-quan-ao/ để sử dụng website.

LƯU Ý QUAN TRỌNG: File db.sql có lệnh xóa và tạo lại các bảng hiện có. Chỉ import khi thiết lập cơ sở dữ liệu mới hoặc khi đã sao lưu dữ liệu; không import lại tùy tiện vì có thể làm mất các sản phẩm, tài khoản và đơn hàng đã phát sinh.

Nếu MySQL trên máy đã đặt mật khẩu riêng cho tài khoản root, thông tin kết nối trong config/db.php cần tương ứng với cấu hình MySQL đó.

FashionStore là đồ án chạy thử trên máy cục bộ bằng XAMPP; không sử dụng thông tin đăng nhập mẫu hoặc trang thiết lập Admin công khai trên máy chủ Internet.
