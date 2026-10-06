---
lang: vi
lang_alt: reference-manuals/monitoring-dam-performance/chapter-11-data-management/
---
# Chương 11 — Thu thập, quản lý dữ liệu và cơ sở dữ liệu

## 11.1 Dữ liệu chỉ có giá trị nếu bạn có thể tìm lại nó sau này

Mục tiêu của quản lý dữ liệu rất đơn giản: mọi số đọc đều được ghi nhận, kiểm
chứng, lưu trữ và có thể truy xuất trong nhiều thập kỷ, cùng với đủ bối cảnh để
một người không có mặt lúc đó có thể diễn giải. Mất dữ liệu là vĩnh viễn; một số
đọc không được lưu cũng giống như chưa từng thực hiện.

## 11.2 Tần suất thu thập

Tần suất được xác định theo tốc độ thay đổi và kế hoạch chương trình
([Chương 4](chapter-04-planning.md)):

- **Trạng thái ổn định** — hàng tháng đến hàng quý đối với các biến đổi chậm.
- **Thi công / lần tích nước đầu tiên** — hàng ngày đến hàng tuần.
- **Sau các sự kiện** — tăng cường, hoặc liên tục thông qua tự động hóa
  ([Chương 9](chapter-09-automated.md)).

## 11.3 Kiểm chứng

Số đọc thô chưa phải là dữ liệu cho đến khi được kiểm tra. Kiểm chứng bao gồm:

- **Kiểm tra miền giá trị** — giá trị đó có khả thi về mặt vật lý không?
- **Tính hợp lý** — nó có phù hợp với xu hướng và mùa vụ không?
- **Đối chiếu chéo** — các thiết bị có tương quan có thống nhất không?
- **Đối chiếu thủ công với tự động** đối với các số đọc điểm.

Dữ liệu xấu phải được đánh dấu, không được lặng lẽ loại bỏ.

## 11.4 Lưu trữ và cơ sở dữ liệu

Một cơ sở dữ liệu giám sát cần ghi lại, đối với mỗi số đọc:

- Định danh và vị trí của thiết bị.
- Mốc thời gian và người đọc.
- Giá trị, đơn vị và độ bất định.
- Bối cảnh môi trường (mực nước hồ, nhiệt độ, lượng mưa).

Ưu tiên các định dạng mở, di động và một hệ thống có lộ trình di chuyển rõ ràng.
Các "hộp đen" độc quyền không thể xuất dữ liệu là một rủi ro lâu dài.

## 11.5 Đường cơ sở như một tài sản được quản lý

Đường cơ sở vận hành đầu ([Chương 2](chapter-02-failure-modes.md)) là một tài
sản được quản lý. Hãy lưu trữ nó một cách rõ ràng để "bình thường" trong tương lai
có thể so sánh với "bình thường" của ngày hôm nay khi đập ngày càng già đi.

## 11.6 Tích hợp với chương trình rộng hơn

Quản lý dữ liệu tốt liên kết các số đọc với kế hoạch giám sát (lý do mỗi thiết bị
tồn tại) và với các kết quả kiểm tra hiện trường (để một bất thường của thiết bị
và một quan sát thực địa có thể được xem xét cùng nhau).

## 11.7 Điểm mấu chốt

- Ghi nhận, kiểm chứng và lưu trữ mọi số đọc với đầy đủ bối cảnh.
- Xác định tần suất theo tốc độ thay đổi, không phải theo sự tiện lợi.
- Đánh dấu dữ liệu xấu; không bao giờ xóa lặng lẽ.
- Sử dụng các hệ thống di động, có thể xuất; coi đường cơ sở như một tài sản lâu dài.
