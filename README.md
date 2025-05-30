"# odoo_consjob"

# Cấu trúc dự án

Dự án bao gồm 6 submodule chính và có thể chia làm 2 nhóm chức năng:

- **Nhóm AsyncTask and MarketMatching:** Bao gồm 3 submodule. Đầu tiên, `vnmarket_cs` là module được triển khai trên hệ thống của các Contractor nhằm mục đích phục vụ việc ghép nối nhà thầu. module `vnmarket_is` được triển khai trên hệ thống tích hợp cho việc giao tiếp giữa các nhà thầu. Cuối cùng, `vnmarket` là module chung, đảm nhiệm các logic nghiệp vụ giống nhau giữa cả hai module đã đề cập. Module `vnmarket_cs` và `vnmarket_is`kế thừa từ `vnmarket`, sau đó tùy theo yêu cầu mà được triển khai thêm.
- **Nhóm Inter-field task mapping:** Bao gồm 3 submodule. Đầu tiên, `vnfield_cs` là module được triển khai trên hệ thống của các Contractor nhằm mục đích phục vụ việc quản lý công việc và phê duyệt cho nội bộ nhà thầu. Ngoài ra, chúng cũng được phát triển cho mục đích tích hợp hoạt động giữa nhiều nhà thầu khác nhau cho cả tính năng quản lý công việc và phê duyệt. module `vnfield_is` được triển khai trên hệ thống tích hợp cho việc giao tiếp giữa các nhà thầu. Cuối cùng, `vnfield` là module chung, đảm nhiệm các logic nghiệp vụ giống nhau giữa cả hai module đã đề cập. Tương tự với nhóm _contractor matching_, `vnfield_cs` và `vnfield_is` cũng được kế thừa từ `vnfield`.

# Odoo store

Các bản release trên Odoo store cho các module tương ứng:

- `vnfield`: [vnfield](https://apps.odoo.com/apps/modules/17.0/vnfield)
- `vnfield_cs`: [vnfield_cs](https://apps.odoo.com/apps/modules/17.0/vnfield_cs)
- `vnfield_is`: [vnfield_is](https://apps.odoo.com/apps/modules/17.0/vnfield_is)

# Architecture:
**AsynTask and MarketMatching**:
- `vnmarket`: [odoo store](https://apps.odoo.com/apps/modules/17.0/vnmarket) [github repo](https://github.com/NietzsLe/odoo_vnmarket)
- `vnmarket_cs`: [odoo store](https://apps.odoo.com/apps/modules/17.0/vnmarket_cs) [github repo](https://github.com/NietzsLe/odoo_vnmarket_cs)
- `vnmarket_is`: [odoo store](https://apps.odoo.com/apps/modules/17.0/vnmarket_is) [github repo](https://github.com/NietzsLe/odoo_vnmarket_is)
**Inter-field task mapping**:
- `vnfield`: [vnfield](https://apps.odoo.com/apps/modules/17.0/vnfield) [github repo](https://github.com/NietzsLe/odoo_vnfield)
- `vnfield_cs`: [vnfield_cs](https://apps.odoo.com/apps/modules/17.0/vnfield_cs) [github repo](https://github.com/NietzsLe/odoo_vnfield_cs)
- `vnfield_is`: [vnfield_is](https://apps.odoo.com/apps/modules/17.0/vnfield_is) [github repo](https://github.com/NietzsLe/odoo_vnfield_is



