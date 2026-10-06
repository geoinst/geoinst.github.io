---
lang: vi
lang_alt: reference-manuals/tailings-dam-safety/chapter-06-pore-pressure/
---
# Chương 6 — Giám sát áp lực nước lỗ rỗng và tiềm năng hóa lỏng

## 6.1 Tại sao áp lực nước lỗ rỗng là tham số trung tâm

Các cơ chế phá hoại bùn thải chủ đạo — **hóa lỏng tĩnh và do động đất** — được
chi phối bởi áp lực nước lỗ rỗng. Khi bùn thải rời rạc, bão hòa mang áp lực nước
lỗ rỗng cao (ứng suất hữu hiệu thấp), chúng có thể mất cường độ một cách thảm
khốc. Vì vậy giám sát áp lực nước lỗ rỗng là nền tảng của giám sát bùn thải.

## 6.2 Các loại áp kế (Piezometer)

| Loại thiết bị | Nguyên lý hoạt động | Ứng dụng tối ưu |
|---------------|---------------------|-----------------|
| **Dây rung (Vibrating-Wire - VW)** | Thay đổi tần số dao động tự nhiên của dây căng | Giám sát tự động liên tục, kết nối datalogger; độ ổn định cao |
| **Khí nén (Pneumatic)** | Áp suất khí cân bằng áp suất nước làm mở van | Vị trí quan trắc thủ công định kỳ, không cần cấp nguồn liên tục |
| **Ống đứng hở (Casagrande)** | Đo trực tiếp mực nước thủy tĩnh trong ống | Đơn giản, trực tiếp; phù hợp đất thấm lớn |
| **Thủy lực (hai ống)** | Cân bằng cột chất lỏng | Khối đắp đập, phương pháp truyền thống |

## 6.3 Các chỉ thị tiềm năng hóa lỏng

Giám sát áp lực nước lỗ rỗng hỗ trợ đánh giá hóa lỏng qua:

- **Tỷ số áp lực nước lỗ rỗng** $r_u = u / \sigma'_v$ — tỷ số giữa áp lực nước
  lỗ rỗng và ứng suất hữu hiệu thẳng đứng ban đầu; $r_u$ cao hoặc tăng lên báo
  hiệu nguy cơ mất cường độ do hóa lỏng.
- **Áp lực nước lỗ rỗng dư** sinh ra trong hoặc sau các sự kiện động đất hoặc gia tải nhanh, đo bởi
  áp kế piezometer có độ nhạy và đáp ứng nhanh.
- **Tương quan với thí nghiệm tại hiện trường** (SPT, CPT, vận tốc sóng cắt) đặc
  trưng cho độ rời rạc của lớp bùn.

!!! warning "Bão hòa màng lọc là yếu tố sống còn"
    Một áp kế piezometer kiểu dây rung hoặc khí nén không được bão hòa hoàn toàn sẽ cho kết quả vô nghĩa. Quy
    trình **bão hòa (saturation)** — loại bỏ toàn bộ bọt khí khỏi đầu lọc xốp và buồng đo — phải được thực hiện
    cẩn thận trước và trong khi lắp đặt ([Dunnicliff Ch. 9](../dunnicliff/index.md)). Một áp kế
    chưa bao giờ được bão hòa đúng cách là một lỗ hổng thầm lặng nguy hiểm trong chương trình quan trắc an toàn đập.

## 6.4 Vị trí đặt

Piezometer được đặt để phát hiện các mode phá hoại của [Chương 2](chapter-02-facilities-and-failures.md):

- **Trong lớp bùn và bãi bùn** để theo dõi mặt nước thấm và các vùng có $r_u$ cao.
- **Tại chân đập đắp** (đặc biệt các đợt đắp cao phương pháp thượng nguồn) để phát
  hiện tích tụ áp lực trong vật liệu yếu nhất.
- **Trong nền móng** nơi có các lớp yếu hoặc có thể hóa lỏng.
- **Nhiều độ sâu** trong một lỗ khoan đơn (nhiều mức / MPBX) để vẽ hồ sơ áp lực
  nước lỗ rỗng theo độ sâu.

## 6.5 Đọc và diễn giải

Các số đọc được chuyển đổi thành **mực piezometric** (cao độ mặt nước tương đương).
Các diễn giải chính:

- **Tăng ổn định không kèm mực hồ tăng** → có thể tắc nghẽn, thấm tăng, hoặc lỗi
  cảm biến.
- **Độ trễ áp lực nước lỗ rỗng** so với mực hồ → chỉ thị khả năng thoát nước và
  thấm thấu.
- **$r_u$ tiệm cận các giá trị dùng trong thiết kế** → lo ngại hóa lỏng.
- **Áp lực dư sau động đất tăng nhanh** → kích hoạt đánh giá ngay lập tức.

## 6.6 Các hỏng hóc thường gặp

- **Không khí xâm nhập / mất bão hòa** → số đọc trôi dạt hoặc không đáp ứng.
- **Nối tắt lỗ khoan** → đọc nhầm vùng.
- **Hư hỏng cáp / điện tử** → lỗi thiết bị tự động phổ biến nhất.

## 6.7 Điểm mấu chốt

- Áp lực nước lỗ rỗng chi phối các phá hoại hóa lỏng chủ đạo.
- Theo dõi tỷ số áp lực nước lỗ rỗng $r_u$ như một chỉ thị hóa lỏng.
- Bão hòa mọi piezometer đúng cách; xác minh nó.
- Đặt thiết bị tại bãi bùn, chân đập và nền móng — nơi các mode bắt nguồn.
