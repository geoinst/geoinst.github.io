---
lang: vi
lang_alt: reference-manuals/practical-rock-engineering/chapter-10-large-underground-caverns/
---

# Chương 10 — Thiết Kế Buồng Khai Đào Ngầm Quy Mô Lớn

## 10.1 Hình Học & Trình Tự Đào Trong Buồng Ngầm Lớn

Các buồng ngầm khai đào quy mô lớn (nhà máy thủy điện ngầm, trạm biến áp ngầm, buồng máy nghiền quặng trong mỏ sâu và các công trình an ninh quốc phòng) có khẩu độ nhịp vượt quá $20 - 35\text{ m}$ và chiều cao tường vách đứng lên tới $40 - 60\text{ m}$.

Ở quy mô hình học khổng lồ này, không thể đào thông toàn bộ tiết diện trong một lần. Việc thi công bắt buộc phải tiến hành theo quy trình đào giật cấp nhiều giai đoạn từ trên đỉnh vòm xuống đáy:

```
Bước 1: Đào hầm gương dẫn đỉnh nóc vòm (Chống giữ ngay bằng neo đỉnh & bê tông phun)
Bước 2: Đào mở rộng hai bên vai vòm (Đạt toàn bộ khẩu độ nhịp; lắp đặt cáp neo dự ứng lực)
Bước 3: Đào hạ tầng giật cấp 1 (Hạ sâu 3-5 m ở giữa; chống giữ tường biên hai bên)
Bước 4: Đào hạ tầng giật cấp 2 đến N (Đào sâu dần xuống dưới, bảo đảm gia cố vách liên tục)
Bước 5: Đào hoàn thiện đáy hầm & Thi công hệ thống hành lang khoan tháo khô
```

---

## 10.2 Định Hướng Trục Buồng Ngầm Theo Ứng Suất & Khe Nứt

Định hướng trục buồng ngầm là quyết định thiết kế quan trọng nhất mang tính sống còn đối với độ ổn định của công trình:

1. **Định Hướng Theo Phương Ứng Suất Ngang Lớn Nhất ($\sigma_H$)**:
   - Trục dọc của buồng ngầm phải được bố trí song song (hoặc lệch không quá $15^\circ - 20^\circ$) so với phương của ứng suất chính ngang lớn nhất ($\sigma_H$).
   - Giải pháp này giảm thiểu tối đa ứng suất nén kích ứng tác dụng vuông góc vào hai bức tường vách đứng cao của buồng ngầm, ngăn ngừa hiện tượng oằn nứt vỡ vách và hạn chế phát triển vùng dẻo sâu.
2. **Định Hướng So Với Các Hệ Thống Khe Nứt Khống Chế**:
   - Trục buồng ngầm tuyệt đối tránh bố trí song song với phương vị của các hệ khe nứt dốc đứng kéo dài hoặc các đới đứt gãy kiến tạo.
   - Nếu một đứt gãy chạy song song với tường vách đứng của buồng ngầm, nó sẽ tạo thành các khối nêm đá nặng hàng vạn tấn có nguy cơ sập trượt khổng lồ, đòi hỏi chi phí cáp neo dự ứng lực cực kỳ tốn kém.

---

## 10.3 Thiết Kế Cáp Neo Dự Ứng Lực Cho Buồng Ngầm Lớn

Các thanh neo đá thông thường (chiều dài $3 - 5\text{ m}$) không đủ chiều sâu để vượt qua vùng phá hoại dẻo nứt nẻ sâu ($6 - 15\text{ m}$) xung quanh buồng ngầm khẩu độ lớn. Bắt buộc phải sử dụng hệ thống cáp neo dự ứng lực chịu lực cao (chiều dài $15 - 25\text{ m}$, sức chịu tải $500 - 1.000\text{ kN}$):

### Các Bộ Phận Cấu Thành Của Cáp Neo:
- **Thân Cáp Neo**: Tập hợp nhiều tao cáp thép cường độ cao 7 sợi (đường kính $15,2\text{ mm}$, tải trọng kéo đứt $260\text{ kN}$ mỗi tao).
- **Đoạn Neo Bầu (Chiều dài ngàm cố định)**: Đoạn cáp dài $5 - 8\text{ m}$ được bơm vữa xi măng hoặc vữa nhựa điền đầy, ngàm chặt vào khối đá nguyên vẹn đàn hồi nằm ngoài vùng biến dạng dẻo.
- **Đoạn Neo Tự Do**: Đoạn cáp được bọc ống nhựa trơn cho phép cáp dãn dài đàn hồi tự do trong quá trình kéo căng tạo ứng suất trước.
- **Đầu Neo & Bản Đệm**: Bản đệm thép kích thước lớn phân bố lực nén cục bộ lên các ụ đệm bê tông phun cốt thép.

$$\text{Tải Trọng Làm Việc Thiết Kế } T_{\text{làm việc}} \le 0,60 - 0,70 T_{\text{kéo đứt}}$$

---

## 10.4 Mạng Lưới Quan Trắc 3D Trong Buồng Ngầm Lớn

Việc đo đạc biến dạng trong suốt quá trình hạ tầng buồng ngầm cung cấp dữ liệu phản hồi quan trọng để kiểm chứng mô hình phần tử hữu hạn và mô hình biên:

| Thiết Bị Quan Trắc | Vị Trí & Bố Trí | Mục Tiêu Quan Trắc Cốt Lõi |
|---------------------|-----------------|-----------------------------|
| **Thiết bị đo biến dạng sâu nhiều điểm (MPBX)** | Chùm hình nan quạt từ đỉnh vòm và hai vách cao (độ sâu $10, 20, 30\text{ m}$) | Đo chiều sâu vùng giãn nở nứt nẻ của khối đá và kiểm tra xem đoạn neo ngàm có nằm trong khối đá bất động hay không |
| **Hộp Đo Ứng Suất Lỗ Khoan (Dây rung)** | Đặt trong các trụ đá ngăn giữa các buồng ngầm kề nhau | Giám sát mức độ tập trung ứng suất trong trụ đá ngăn giữa buồng gian máy và buồng máy biến áp |
| **Cảm Biến Đo Tải Trọng Đầu Neo (Load Cell)** | Lắp đặt dưới bản đệm đầu neo cáp | Theo dõi liên tục xem biến dạng khối đá có làm căng cáp quá tải dẫn đến nguy cơ đứt cáp đột ngột hay không |
| **Mốc Đo Chuyển Vị Bề Mặt (RTS)** | Lưới mốc phản xạ 3D trên đỉnh vòm và vách đứng | Đo véc-tơ chuyển vị co hẹp 3D sau mỗi đợt nổ mìn hạ các tầng bên dưới |

---

## 10.5 Thuật ngữ Đối chiếu Chuẩn hóa

| Thuật ngữ Tiếng Anh | Thuật ngữ Tiếng Việt Chuẩn hóa | Định nghĩa Kỹ thuật |
|---------------------|--------------------------------|----------------------|
| Underground cavern | Buồng ngầm quy mô lớn | Không gian ngầm đào trong đá có khẩu độ nhịp và chiều cao tường lớn |
| Pre-stressed cablebolt | Cáp neo dự ứng lực | Cáp thép cường độ cao được kéo căng trước để ép chặt khối đá |
| Free length | Đoạn tự do của neo | Đoạn thân neo không dính bám cho phép dãn dài đàn hồi khi căng kéo |
| Bond length | Đoạn neo bầu / Chiều dài đoạn ngàm | Đoạn neo ngàm chặt vào đá nhờ vữa để truyền lực vào khối đá ổn định |
| Sequential benching | Đào hạ tầng giật cấp | Phương pháp đào từ trên xuống chia thành các tầng ngang tuần tự |
