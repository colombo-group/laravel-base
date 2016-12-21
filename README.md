# Laravel Base

## Phiên bản

- [Laravel 5.3](https://laravel.com/docs/5.3)
- [Bootstrap v4](https://v4-alpha.getbootstrap.com)

## Mục tiêu

- Sử dụng được laravel 5.3 và hiểu được các tư tưởng quan trọng nhất trong laravel.
- Làm quen với Bootstrap 4 với các concept về html5/css3 rõ ràng hơn.
- Sử dụng các tooldev trong laravel (composer, gulp, webpack, ...)

## Tổng quan

- Xây dựng 1 trang dạng CMS, bao gồm người dùng và blog là 2 phần chính
- Phần người dùng có phân quyền : `Registered`, `User`, `Admin`
 - `Admin` là người có tất cả quyền
 - `User` là người có thể đăng nhập và viết bài
 - `Registered` là người có thể xem một số bài giới hạn, có thể comment

- Phần blog là các bài viết của User, Admin. Tính năng comment được dùng cho toàn bộ người dùng đã đăng nhập.

## Chi tiết

### Level 1

- Tính năng:
 - Đăng ký : đăng ký bằng 3 thông tin cơ bản `tên`, `email`, `password`. Sau khi đăng ký có thể đăng nhập được luôn ko cần active. Sau khi đăng ký người dùng có quyền `User`.
 - Đăng nhập : chỉ đăng nhập bằng email
 - Trang quản trị : hiển thị 1 thông báo chào mừng
 - Chỉnh sửa thông tin : chỉnh sửa thông tin cơ bản và thêm `giới tính`, `ngày sinh`, `địa chỉ`, `slogan`.
 - Quản lý danh sách user : chỉ là danh sách có phân trang

- Yêu cầu:
 - Trang quản trị, quản lý danh sách phải có đường dẫn bắt đầu bằng `admin/` - _gọi là khu vực admin và chỉ được sử dụng bởi admin_
 - Trang Đăng ký/Đăng nhập/Chỉnh sửa thông tin thì ko nằm trong khu vực admin.
 - Giao diện sử dụng bootstrap 4
 - Không code trực tiếp js/css trực tiếp trong public(sử dụng gulp)

- Mục tiêu kiến thức :
 - Làm quen laravel 5.3
 - Làm quen bootstrap4
 - Cách phân chia ứng dụng thành 2 khu vực khác nhau tạm gọi là `admin`/`frontend`

### Level 2
_Tạo 1 branch có tên level1 từ master sau khi code xong `Level 1`_
- Tính năng:
 - A
 - B

