---
lang: vi
lang_alt: applications/tunnels/
---

# Thiết Bị Quan Trắc Hầm

## Mục tiêu

Quan trắc chuyển động đất xung quanh đào hầm, sự hội tụ của lớp lót, và thay đổi áp lực lỗ rỗng trong thi công — bảo vệ cả tiết diện hầm và các công trình lân cận phía trên.

---

## Tham chiếu chương toàn diện từ các tài liệu tham khảo

### Từ Dunnicliff — Geotechnical Instrumentation for Monitoring Field Performance
| Chapter | Title | Application to Tunnel Instrumentation |
|---------|-------|----------------------------------------|
| **Ch 1** | Thiết bị quan trắc địa kỹ thuật: Tổng quan | Tầm quan trọng của quan trắc hầm, hậu quả sập |
| **Ch 2** | Ứng xử của đất và đá | Ứng xử khối đá, đất siết, nổ vỡ đá |
| **Ch 3** | Lợi ích của việc sử dụng thiết bị quan trắc địa kỹ thuật | Kiểm chứng thiết kế, an toàn thi công, hợp đồng |
| **Ch 4** | Phương pháp tiếp cận có hệ thống để lập kế hoạch chương trình quan trắc | Quy trình lập kế hoạch 20 bước cho dự án hầm |
| **Ch 8** | Cảm biến biến đổi và thu thập dữ liệu | Cảm biến hội tụ, hệ thống tự động |
| **Ch 9** | Đo áp lực nước ngầm | Áp lực hạ mực nước, piezometer (đầu đo áp lực nước) tại mặt hầm |
| **Ch 12** | **Đo biến dạng** | **Chính** — Hội tụ, extensometer (đầu đo biến dạng), inclinometer (đầu đo nghiêng) |
| **Ch 13** | Đo tải trọng và biến dạng | Tải trọng bulông đá, ứng suất lót, telltale |
| **Ch 17** | Lắp đặt thiết bị | Đặc thù hầm: khoan từ hầm, không gian hạn chế |
| **Ch 18** | Thu thập, xử lý, trình bày, diễn giải | Quan trắc hội tụ thời gian thực, hệ thống cảnh báo |
| **Ch 23** | **Đào ngầm** | **Chương chính cho hầm** — hội tụ, bulông đá, nước ngầm, áp lực mặt hầm |

### Từ Das — Principles of Foundation Engineering (7th Ed)
| Chapter | Application |
|---------|-------------|
| **Ch 13** | Áp lực đất ngang — thiết kế lót hầm |
| **Ch 15** | Ổn định sườn dốc — sườn dốc cửa hầm, lún bề mặt |

### Từ Das — Principles of Geotechnical Engineering (7th Ed)
| Chapter | Application |
|---------|-------------|
| **Ch 12** | Sức kháng cắt — thông số cường độ khối đá |
| **Ch 15** | Ổn định sườn dốc — ổn định cửa hầm, rãnh lún bề mặt |

### Từ Murthy — Advanced Foundation Engineering
| Topic | Application |
|-------|-------------|
| Lớp lót hầm | Thiết kế lót phân đoạn, mối nối phân đoạn |
| Quan trắc TBM | Áp lực khiên, khớp nối, khớp nối |

### Từ Benerjee & Butterfield — Advanced Geotechnical Analyses
| Topic | Application |
|-------|-------------|
| Mô hình hóa số | FEM/DEM cho trình tự đào hầm |

### Từ Field Methods for Geologists and Hydrologists
| Topic | Application |
|-------|-------------|
| Địa chất cấu trúc | Lập bản đồ bất liên tục, phân loại khối đá |

### Từ Encyclopedia of Field and General Geology
| Topic | Application |
|-------|-------------|
| Phương pháp đào hầm | Khoan-nổ, TBM, NATM, đào tuần tự |

---

## Mảng thiết bị điển hình cho thiết bị quan trắc hầm

| Instrument | Purpose | Dunnicliff Chapter | Representative Instrument |
|------------|---------|-------------------|------------------------|
| **Mảng hội tụ / extensometer thước** | Quan trắc thu hẹp tiết diện hầm | Ch 12, 23 | Tape extensometers, convergence arrays |
| **Extensometer lỗ khoan đa điểm (MPBX)** | Dịch chuyển khối đá phía trên vòm | Ch 12, 23 | MPBX extensometers, wireless |
| **Inclinometer (bề mặt/cửa hầm)** | Phát hiện rãnh lún bề mặt | Ch 12, 23 | MEMS inclinometers, IPI arrays |
| **Piezometer** | Áp lực hạ mực nước gần mặt hầm | Ch 9, 23 | VW piezometers, wireless |
| **Load cell bulông đá** | Quan trắc tải trọng neo/bulông | Ch 13, 23 | VW load cells, strain gages |
| **Đồng hồ đo hội tụ** | Hội tụ lót thời gian thực | Ch 12, 23 | Convergence meters, wireless |
| **Điện trở biến dạng bulông đá** | Quan trắc tải trọng bulông | Ch 13 | VW strain gages, wireless |
| **Tế bào áp lực (NATM)** | Áp lực đất lên lót | Ch 10, 23 | VW pressure cells |
| **Crackmeter / jointmeter** | Độ mở mối nối phân đoạn | Ch 12, 23 | Crackmeters, jointmeters |
| **Inclinometer (khiên TBM)** | Khớp nối/căn chỉnh TBM | Ch 12 | MEMS tilt sensors |
| **wireless mesh radio** | Dữ liệu từ hầm về cổng mặt đất | Ch 8, 18 | wireless mesh + surface gateway |

---

## Hướng dẫn lắp đặt (từ Dunnicliff Ch 12, 17, 23)

### Quan trắc hội tụ
- **Loại mảng**: Extensometer thước, đồng hồ đo hội tụ, MPBX
- **Vị trí**: Vòm, đường đứng lò (springline), đáy lót (invert)
- **Tần suất**: Hàng ngày (đào), hàng tuần (thi công), hàng tháng (vận hành)

### Lắp đặt extensometer (MPBX)
- **Độ sâu neo**: Nhiều mỏ neo tại các độ sâu phủ đá khác nhau
- **Lắp đặt**: Từ vòm hầm / khoan từ bề mặt
- **Đầu tham chiếu**: Vị trí ổn định ngoài vùng ảnh hưởng hầm

### Lắp đặt piezometer
- **Vị trí**: Phía trước mặt hầm, tại mặt hầm, phía sau lót
- **Loại**: Piezometer VW cho đọc từ xa
- **Quan trắc hạ mực nước**: Thượng lưu/hạ lưu hầm

### Quan trắc bulông đá
- **Load cell**: Lắp tại đầu bulông
- **Điện trở biến dạng**: Dán vào thân bulông
- **Telltale**: Cho độ dài kéo dài bulông dài

---

## Hướng dẫn diễn giải dữ liệu (từ Dunnicliff Ch 18, 23)

| Parameter | Normal Range | Alert Level | Critical Level | Reference |
|-----------|--------------|-------------|----------------|-----------|
| Tốc độ hội tụ | < 2 mm/ngày | > 5 mm/ngày | > 10 mm/ngày | Ch 23 |
| Tốc độ lún vòm | < 2 mm/ngày | > 5 mm/ngày | > 10 mm/ngày | Ch 23 |
| Tổn hao tải trọng bulông đá | < 10% | > 20% | > 30% | Ch 13 |
| Thay đổi áp lực lỗ rỗng | Đường cơ sở | 2× cơ sở | > giá trị thiết kế | Ch 9, 23 |
| Tốc độ tổn hao tải trọng bulông đá | < 5%/tháng | > 10%/tháng | > 20%/tháng | Ch 13 |

---

## Quan Trắc Tự Động Cho Hầm (Dunnicliff Ch 18, Ch 23)

| System | Function | Implementation |
|--------|----------|-------------------|
| **Hội tụ thời gian thực** | Quan trắc vòm/springline liên tục | wireless convergence sensors |
| **Quan trắc áp lực mặt hầm** | Áp lực khiên TBM, hạ mực nước | wireless piezometers |
| **Quan trắc bulông đá** | Tải trọng + biến dạng bulông | VW load cells + strain gages |
| **Cảnh báo tự động** | Vượt ngưỡng | cloud platform |
| **Tích hợp dữ liệu TBM** | Áp lực khiên, khớp nối | wireless mesh + TBM interface |

---

## Trang liên quan
- [Chương 23 Dunnicliff](../reference-manuals/dunnicliff/chapter-14-applications.md)
- [GTI Doctor — Hỏi về quan trắc hầm](../gti-doctor.md)

---

*Nguồn: Tổng hợp từ Dunnicliff (616 chunks), Das Foundation (817 pp), Das Geotechnical (683 pp), Murthy (821 pp), Benerjee & Butterfield (394 pp), Field Methods (405 pp), Encyclopedia (952 pp), NCHRP Synthesis 89, và các tài liệu tham khảo hiện trường.*
