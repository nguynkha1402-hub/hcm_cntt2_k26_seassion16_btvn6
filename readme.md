## Bản đặc tả không gian cộng tác (README)
-Cấu trúc lưu trữ (Hybrid):

- Git Repo (Code): Lưu ``src/sensors/`` và `.gitignore`.
- Cloud Drive (Tài liệu): Lưu `investor-reports/` và `partner-specs/`.  

-Kênh giao tiếp:

- Thiết lập kênh` #dev-sensors` (code) và `#alerts-hardware` (lỗi).
- Quản lý Task: Sử dụng tính năng "Create Task/Issue" tích hợp trong app chat (Slack/Teams) để chuyển trực tiếp tin nhắn báo cáo lỗi thành công việc có Assignee và Deadline.  

-Phân quyền & Bảo mật:

- Nhà đầu tư: Quyền Viewer với thư mục báo cáo. 
- Đối tác: Quyền Commenter  với thư mục tài liệu thiết bị. 
- File ```.env```: Bắt buộc liệt kê trong `.gitignore` để không đẩy lên kho code chung. Chia sẻ mật khẩu cục bộ qua trình quản lý mật khẩu. 
- Bàn giao: Sử dụng tính năng Transfer Ownership trên Cloud Drive và Git Repo để chuyển giao toàn quyền sở hữu cho người nhận khi kết thúc dự án.

## Kiểm thử 
- Nếu xóa mất code: Mở Terminal tại thư mục gốc, chạy lệnh `git restore src/sensors` để khôi phục mã nguồn về trạng thái nguyên vẹn gần nhất.
- Nếu xóa nhầm tài liệu trên Cloud Drive: Truy cập Thùng rác, tìm thư mục `sensors` và chọn Restore để lấy lại kèm nguyên trạng thái phân quyền.   