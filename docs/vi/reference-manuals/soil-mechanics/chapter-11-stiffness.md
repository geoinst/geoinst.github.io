---
lang: vi
lang_alt: reference-manuals/soil-mechanics/chapter-11-stiffness/
---
# Chương 11 — Độ cứng & Ứng suất–Biến dạng

## 11.1 Vì sao độ cứng quan trọng

**Độ cứng** — mức đất biến dạng khi ứng suất thay đổi — chi phối **lún**, **phân bố tải**
giữa các cấu kiện kết cấu và **dịch chuyển** quanh hố đào. Nó được đo bằng một **mô đun**, và
khác với cường độ, nó **rất phi tuyến** và **phụ thuộc biến dạng**.

## 11.2 Các thông số đàn hồi

Ở biến dạng nhỏ, đất được mô tả bằng:

- **Mô đun Young** $E$ — độ dốc ứng suất–biến dạng theo hướng chất tải.
- **Hệ số Poisson** $\nu$ — tỷ số biến dạng ngang trên biến dạng dọc (thường 0,2–0,5; 0,5
  cho không thoát nước).
- **Mô đun cắt** $G = E / [2(1+\nu)]$ — khả năng kháng biến dạng cắt, thường là thông số hữu
  ích nhất cho bài toán động và biến dạng nhỏ.
- **Mô đun khối** $K$ — khả năng kháng biến đổi thể tích.

## 11.3 Phi tuyến và mức biến dạng

Độ cứng của đất **giảm** khi biến dạng tăng:

- **Biến dạng rất nhỏ** ($< 0,001\%$) — độ cứng lớn nhất $G_0$ hoặc $E_0$, đo bằng **phương
  pháp địa chấn** (bender element, CPT địa chấn, MASW).
- **Biến dạng nhỏ** — liên quan móng máy và tải động.
- **Biến dạng làm việc** ($0,01–1\%$) — liên quan hầu hết lún móng; độ cứng là một phần của
  $G_0$.
- **Biến dạng lớn** — gần phá hoại; liên quan ổn định.

Thiết kế phải dùng mô đun **phù hợp mức biến dạng** của bài toán — lỗi phổ biến là dùng một
"mô đun" duy nhất cho mọi trường hợp.

## 11.4 Xác định giá trị mô đun

- **Trong phòng** — thí nghiệm ba trục hoặc oedometer cho $E$ hoặc mô đun nén trong một dải
  biến dạng.
- **Hiện trường** — pressuremeter, dilatometer, thí nghiệm bàn nén và **phương pháp địa
  chấn** cho giá trị tại chỗ, thường tốt hơn vì tránh xáo trộn mẫu.
- **Tương quan** — với SPT $N$ hoặc sức kháng mũi CPT, hữu ích để ước lượng ban đầu.

## 11.5 Các điểm then chốt cần ghi nhớ

- **Độ cứng chi phối lún** và phân bố tải.
- Độ cứng đất **phi tuyến và phụ thuộc biến dạng** — $G_0$ ở biến dạng nhỏ, thấp hơn nhiều
  gần phá hoại.
- Dùng mô đun **phù hợp mức biến dạng** của bài toán.
- **Phương pháp địa chấn** cho mô đun biến dạng nhỏ; **thí nghiệm hiện trường** cho giá trị
  làm việc.
- **Tương quan** với SPT/CPT là điểm khởi đầu, không thay thế thí nghiệm.
