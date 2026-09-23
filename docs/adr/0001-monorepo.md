# ADR 0001: Project đang sử dụng Monorepo
## Quyết định:

Dự án sử dụng Monorepo để quản lý toàn bộ dự án Clinic Booking trong một Git repo
Frontend Next.js và Backend ASP.NET Core được tổ chức riêng trong thư mục apps/ với 2 thư mục /api và /web
Cách tổ chức này giúp đội có thể quản lý mã nguồn fe và be tập trung cùng một repository
Các thay đổi liên quan giữa be và fe có thể được theo dõi và review dễ dàng hơn
Tài liệu và cấu hình dùng chung có thể quản lý tập trung
Docker compose có thể được sử dụng chung để có thể quản lý Postgres và Redis vervices 
Mô hình này phù hợp với quy mô hiện tại của dự án và giúp giảm sự phức tạp trong quá trình phát triển 
FE và BE cũng có thể được triển khai và phát triển độc lập khi cần 