Task Tổng Hợp 01

# Chủ đề tổng hợp: Laravel: Auth Custom, Routing, Controllers, Validation, Eloquent Polymorphic Relationships, Export, Import, Policies, Gates, Facades, Helpers, Component, Session, Form Requests, Error Handling, Logging, Exception, Artisan Console, Crontab (Linux), Queues, Task Scheduling, Cache

# Yêu cầu:
- Xây dựng một trang web có sitemap như sau
```
/
├───admin/
│   ├───login/
│   ├───register/
│   ├───forget_password/
│   ├───logout/
│   ├───post/
│   │   ├───create/
│   │   ├───edit/
│   │   ├───delete/
│   │   └───detail/
│   ├───media/
│   │   ├───upload/
│   │   ├───edit/
│   │   ├───delete/
│   │   └───detail/
│   ├───comment/
│   │   ├───create/
│   │   ├───edit/
│   │   └───delete/
│   ├───export/
│   ├───import/
│   └───rule/
├───login/
├───register/
├───forget_password/
├───logout/
├───mypage/
│   ├───post/
│   ├───like/
│   └───profile/
└───post/
    └───detail/
```
- Chức năng chính đăng bài, thảo luận và like bài viết trong đó.
	+ Post cần có các field như title, url, content (sử dụng ckeditor), thumbnail.
	+ Comment cần có field như content (sử dụng ckeditor), image.
	+ Comment có thể thảo luận cho post và có thể trả lời cho các comment khác.
- Chức năng mypage, profile
	+ Trang like hiển thị các bài đã like
	+ Trang profile: hiển thị danh sách các comment của user đó và danh sách ai đã like bài của mình.
	+ Trang post để user đăng bài viết
- Chức năng quản lý Media (Media có thể lưu nhiều ảnh của Post và Comment)
- Chức năng đăng nhập user và admin sử dụng riêng biệt. (không chung bảng users)
- Chức năng export các user và các bài viết ra định dạng csv và excel (lưu ý bỏ 2 cột ngày create và update)
- Chức năng import các user từ định dạng csv
- Trang admin rule dùng để phân quyền cho user
	+ được/không được phép post bài
	+ được/không được phép comment bài
# Yêu cầu khác:
- Sử dụng Component để tạo form input
- Sử dụng session database
- Sử dụng Form Requests
- sử dụng Error Handling, Logging sau đó tạo custom Logging hoặc Exception custom, để bắt các lỗi vào file log_mypage riêng biệt cho chức năng của trang mypage.
- Tạo command backup bảng user định kỳ mỗi ngày, xuất định dạng csv, gửi mail đến admin khi có bảng backup mới.
- Thiết lập crontab trên linux chạy schedule mỗi phút.
- Áp dụng Cache cho toàn site
# Yêu cầu giao diện
- Sử dụng giao diện phù hợp của Bootstrap https://getbootstrap.com/docs/4.5/getting-started/introduction/
