---
lang: vi
lang_alt: reference-manuals/monitoring-dam-performance/chapter-06-piezometers/
---
# Chương 6 — Áp kế (Piezometer) & Giám sát Áp lực Nước Lỗ rỗng

## 6.1 Tại sao áp lực nước lỗ rỗng là trọng tâm

Áp lực nước lỗ rỗng (pore water pressure) — áp lực của nước bên trong lỗ rỗng của đất, khe nứt của đá, hoặc khối bê tông — là nguyên nhân trực tiếp chi phối ứng suất hữu hiệu, lưu lượng thấm, độ ổn định mái dốc, và lực đẩy nổi (uplift). Đây là một trong những đại lượng địa kỹ thuật quan trọng nhất được giám sát tại các công trình đập và hồ chứa. Sự gia tăng bất thường của áp lực nước lỗ rỗng có thể báo trước cả hiểm họa xói ngầm (piping) lẫn nguy cơ trượt lở mái dốc.

## 6.2 Các loại áp kế (Piezometer)

| Loại thiết bị | Nguyên lý hoạt động | Phạm vi ứng dụng tối ưu |
|---------------|---------------------|--------------------------|
| **Dây rung (Vibrating-Wire - VW)** | Thay đổi tần số dao động tự nhiên của dây thép căng | Giám sát tự động dài hạn, kết nối datalogger; độ ổn định cao |
| **Khí nén (Pneumatic)** | Áp lực khí cân bằng với áp lực nước làm mở màng van | Vị trí quan trắc thủ công định kỳ, độ trễ thấp, không cần nguồn điện tại chỗ |
| **Ống đứng hở (Open Standpipe / Casagrande)** | Đo trực tiếp cao trình mực nước thủy tĩnh trong ống | Đơn giản, độ tin cậy cơ học cao; thích hợp cho đất thấm lớn |
| **Thủy lực hai ống (Twin-Tube Hydraulic)** | Cân bằng cột chất lỏng qua hệ hai ống tuần hoàn | Đắp đất thân đập, có thể súc rửa bọt khí định kỳ |

!!! warning "Bão hòa màng lọc là yếu tố sống còn"
    Một áp kế piezometer kiểu dây rung hoặc khí nén không được bão hòa hoàn toàn sẽ cho kết quả đo sai lệch nghiêm trọng. Quy trình **bão hòa (saturation / de-airing)** —
    loại bỏ toàn bộ không khí khỏi đầu lọc xốp và buồng đo — phải được thực hiện tỉ mỉ
    trước và trong khi lắp đặt. Một áp kế chưa bao giờ được bão hòa đúng cách sẽ tạo ra dữ liệu giả tạo hoặc khoảng trống
    thầm lặng nguy hiểm trong chương trình giám sát an toàn đập. (Xem chi tiết tại [Dunnicliff Ch. 9](../dunnicliff/index.md)).

## 6.3 Vị trí lắp đặt

Vị trí lắp đặt Piezometer tuân theo các mode phá hoại (failure modes):

- **Hạ lưu của lõi đập và tường cắt** để phát hiện sự tích tụ thấm.
- **Trong nền móng** bên dưới và hạ lưu đập.
- **Tại bề mặt thấm (phreatic surface)** để theo dõi đường thấm qua đập đất.
- **Tại chân đập bê tông** để giám sát lực đẩy nổi (uplift).

Nhiều độ sâu tại một lỗ khoan duy nhất (kiểu nhiều tầng hoặc MPBX) cho thấy
biểu đồ áp lực nước lỗ rỗng theo phương thẳng đứng.

## 6.4 Các yếu tố thiết yếu khi lắp đặt

- Khoan và lót ống lỗ khoan; tránh làm nhờn (smearing) đất xung quanh.
- Đặt đầu đo vào tầng địa chất quan tâm với các gói lọc (filter packs) thích hợp.
- Đắp lại và trám kín để ngăn nước chạy tắt (short-circuiting) dọc theo lỗ khoan.
- Bão hòa hoàn toàn đầu đo VW và pneumatic.
- Ghi lại chi tiết lắp đặt — độ sâu, tầng địa chất, hướng, ngày tháng — vào hồ sơ vĩnh viễn.

## 6.5 Đọc và diễn giải

Các số đọc thường được chuyển đổi thành **cột áp Piezometric** (piezometric head) (cao độ của
mặt nước tương đương). Các diễn giải chính:

- **Tăng liên tục mà không có sự dâng mực hồ** → có thể tắc nghẽn, tăng thấm, hoặc lỗi cảm biến.
- **Độ trễ áp lực nước lỗ rỗng** so với mực hồ → cho thấy đường thoát nước và tính thấm.
- **Vượt quá đường phreatic được dùng trong thiết kế** → lo ngại về ổn định.

## 6.6 Các sự cố thường gặp

- **Xâm nhập khí / mất bão hòa** → số đọc trôi dạt hoặc không phản hồi.
- **Chạy tắt lỗ khoan** → đọc sai vùng.
- **Hư hại do đóng băng** → mất dữ liệu mùa đông ở khí hậu lạnh.
- **Hư hỏng điện / cáp** → lỗi phổ biến nhất của thiết bị tự động.

## 6.7 Điểm mấu chốt

- Áp lực nước lỗ rỗng chi phối thấm, ổn định mái dốc, và lực đẩy nổi — hãy giám sát cẩn thận.
- Bão hòa đầu đo VW và pneumatic đúng cách; một Piezometer chưa bão hòa là vô dụng.
- Đặt thiết bị tại nơi các mode phá hoại xuất hiện; sử dụng lắp đặt nhiều tầng.
- Diễn giải dưới dạng cột áp Piezometric và so sánh với bề mặt phreatic thiết kế.
