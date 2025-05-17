"# odoo_consjob"

# Cấu trúc dự án

Dự án bao gồm 6 submodule chính và có thể chia làm 2 nhóm chức năng:

- **Nhóm contractor matching:** Bao gồm 3 submodule. Đầu tiên, `vnmarket_cs` là module được triển khai trên hệ thống của các Contractor nhằm mục đích phục vụ việc ghép nối nhà thầu. module `vnmarket_is` được triển khai trên hệ thống tích hợp cho việc giao tiếp giữa các nhà thầu. Cuối cùng, `vnmarket` là module chung, đảm nhiệm các logic nghiệp vụ giống nhau giữa cả hai module đã đề cập. Module `vnmarket_cs` và `vnmarket_is`kế thừa từ `vnmarket`, sau đó tùy theo yêu cầu mà được triển khai thêm.
- **Nhóm task management và approval:** Bao gồm 3 submodule. Đầu tiên, `vnfield_cs` là module được triển khai trên hệ thống của các Contractor nhằm mục đích phục vụ việc quản lý công việc và phê duyệt cho nội bộ nhà thầu. Ngoài ra, chúng cũng được phát triển cho mục đích tích hợp hoạt động giữa nhiều nhà thầu khác nhau cho cả tính năng quản lý công việc và phê duyệt. module `vnfield_is` được triển khai trên hệ thống tích hợp cho việc giao tiếp giữa các nhà thầu. Cuối cùng, `vnfield` là module chung, đảm nhiệm các logic nghiệp vụ giống nhau giữa cả hai module đã đề cập. Tương tự với nhóm _contractor matching_, `vnfield_cs` và `vnfield_is` cũng được kế thừa từ `vnfield`.
