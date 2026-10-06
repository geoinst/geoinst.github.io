---
lang: vi
lang_alt: applications/slope-stability/
---

# Quan Trắc Ổn Định Sườn Dốc

## Mục tiêu

Phát hiện sự khởi phát của chuyển động sườn dốc trước khi sập, xác định bề mặt trượt cắt, và định lượng tốc độ chuyển động để phục vụ cảnh báo sớm và khắc phục.

---

## Tham chiếu chương toàn diện từ các tài liệu tham khảo

### Từ Dunnicliff — Geotechnical Instrumentation for Monitoring Field Performance
| Chapter | Title | Application to Slope Stability |
|---------|-------|--------------------------------|
| **Ch 1** | Thiết bị quan trắc địa kỹ thuật: Tổng quan | Tầm quan trọng của quan trắc sườn dốc, hậu quả khi sập |
| **Ch 2** | Ứng xử của đất và đá | Sức kháng cắt, cơ chế sập, ứng xử đất/đá |
| **Ch 3** | Lợi ích của việc sử dụng thiết bị quan trắc địa kỹ thuật | Cảnh báo sớm, kiểm chứng thiết kế, bảo vệ pháp lý |
| **Ch 4** | Phương pháp tiếp cận có hệ thống để lập kế hoạch chương trình quan trắc | Quy trình lập kế hoạch 20 bước dành riêng cho sườn dốc |
| **Ch 9** | Đo áp lực nước ngầm | Piezometer (đầu đo áp lực nước) cho áp lực lỗ rỗng kích hoạt sập |
| **Ch 12** | Đo biến dạng | Inclinometer (đầu đo nghiêng), extensometer (đầu đo biến dạng), tiltmeter (cảm biến góc nghiêng), hệ thống lún |
| **Ch 17** | Lắp đặt thiết bị | Khoan, bơm vữa, lắp đặt ống casing trong sườn dốc |
| **Ch 18** | Thu thập, xử lý, trình bày, diễn giải | Tần suất thu thập dữ liệu, hệ thống tự động, diễn giải |
| **Ch 19** | Hố móng có chống giữ | Tải trọng thanh chống, biến dạng tường, chuyển động đất, nước ngầm |
| **Ch 22** | **Sườn dốc đào và tự nhiên** | **Chương chính cho sườn dốc** — inclinometer, piezometer, tiltmeter, khảo sát bề mặt |

### Từ Kỹ thuật móng: Tài liệu tham khảo thuộc phạm vi công cộng (USACE / FHWA)
| Chapter | Title | Application |
|---------|-------|-------------|
| **Ch 13** | Ổn định mái dốc | Sườn dốc vô hạn/hữu hạn, phương pháp lát cắt, hệ số an toàn |
| **Ch 10** | Áp lực đất ngang | Rankine/Coulomb, áp lực chủ động/bị động lên sườn dốc |
| **Ch 11** | Tường chắn & Tường đất có cốt (MSE) | Kết cấu ổn định tại chân mái dốc |
| **Ch 12** | Tường cừ & Hố đào chống đỡ | Chống đỡ hố đào trên mái dốc |

### Từ Cơ học đất & Địa kỹ thuật: Tài liệu tham khảo thuộc phạm vi công cộng (USACE / FHWA)
| Chapter | Title | Application |
|---------|-------|-------------|
| **Ch 6** | Thấm & Lưới thấm | Lực thấm, tiêu thoát nước mái dốc |
| **Ch 7** | Ứng suất hữu hiệu & Áp lực nước lỗ rỗng | Ảnh hưởng áp lực lỗ rỗng lên ứng suất hữu hiệu |
| **Ch 10** | Sức kháng cắt | Mohr-Coulomb, thí nghiệm ba trục, CU/CD, thông số áp lực lỗ rỗng |
| **Ch 13** | Đất có vấn đề | Đất trương nở và đất sụt trên mái dốc |

---

## Mảng thiết bị điển hình cho ổn định sườn dốc

| Instrument | Purpose | Dunnicliff Chapter | Representative Instrument |
|------------|---------|-------------------|------------------------|
| **Mảng inclinometer tại chỗ (IPI)** | Hồ sơ liên tục chuyển động ngang | Ch 12, 22 | MEMS IPI, wireless IPI |
| **Piezometer dây rung (vibrating-wire)** | Áp lực nước lỗ rỗng kích hoạt sập | Ch 9, 22 | VW piezometers, wireless piezometer nodes |
| **Tiltmeter bề mặt** | Phát hiện mép trên của khối chuyển động | Ch 12, 22 | MEMS tiltmeters, wireless tilt arrays |
| **Điểm khảo sát bề mặt / GPS** | Quan trắc dịch chuyển bề mặt | Ch 12, 22 | Locator One GNSS, wireless mesh radio |
| **Crackmeter / jointmeter** | Độ mở khe nứt/khe nối rời rạc | Ch 12 | Crackmeters, jointmeters |
| **wireless mesh radio** | Đưa dữ liệu cảm biến về cổng cảnh báo | Ch 8, 18 | wireless mesh radio |

---

## Hướng dẫn lắp đặt (từ Dunnicliff Ch 9, 12, 17, 22)

### Lắp đặt inclinometer
- Ống casing: ABS hoặc nhôm, có rãnh (tiêu chuẩn 4 rãnh)
- Bơm vữa: Vữa xi măng-bentonit, phương pháp tremie
- Số đọc ban đầu: Thiết lập đường cơ sở trong vòng 24 giờ
- Tần suất đọc: Hàng ngày (thi công), hàng tuần (quan trắc), hàng tháng (dài hạn)

### Lắp đặt piezometer
- Đầu lọc: Bão hòa, tương thích với lớp địa tầng
- Làm kín: Bentonit phía trên/dưới vùng lọc
- Bão hòa: Piezometer VW theo quy trình Ch 9
- Định tuyến cáp: Được bảo vệ, giảm ứng suất kéo

### Lắp đặt tiltmeter
- Gá lắp: Tấm bê tông ổn định hoặc nền đá
- Hướng: Vuông góc với hướng chuyển động dự kiến
- Bù nhiệt: Bắt buộc với MEMS

---

## Hướng dẫn diễn giải dữ liệu (từ Dunnicliff Ch 18, 22)

| Parameter | Threshold/Action Level | Reference |
|-----------|------------------------|-----------|
| Tốc độ dịch chuyển inclinometer | > 5 mm/ngày = cảnh báo; > 20 mm/ngày = sơ tán | Ch 22 |
| Tăng áp lực lỗ rỗng | > 80% giá trị thiết kế = cảnh báo | Ch 22 |
| Tốc độ nghiêng | > 0,1°/ngày = cảnh báo | Ch 22 |
| Tốc độ mở crackmeter | > 1 mm/ngày = cảnh báo | Ch 22 |

---

## Trang liên quan
- [Chương 22 Dunnicliff](../reference-manuals/dunnicliff/chapter-14-applications.md)
- [GTI Doctor — Hỏi về quan trắc sườn dốc](../gti-doctor.md)

---

*Nguồn: Tổng hợp từ Dunnicliff (616 chunks), Foundation Engineering (USACE/FHWA, phạm vi công cộng), Soil Mechanics (USACE/FHWA, phạm vi công cộng), NCHRP Synthesis 89, và các tài liệu tham khảo hiện trường.*
