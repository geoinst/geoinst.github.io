---
lang: vi
lang_alt: reference-manuals/dunnicliff/chapter-05-uncertainty/
---

# Chương 5 — Độ không đảm bảo đo và hệ thống thu thập dữ liệu

## 5.1 Mọi phép đo hiện trường đều có độ không đảm bảo

Không có bất kỳ phép đo địa kỹ thuật nào là tuyệt đối chính xác. Việc hiểu rõ, kiểm soát và định lượng được **độ không đảm bảo đo (Measurement Uncertainty)** là ranh giới phân biệt giữa một chương trình quan trắc khoa học tin cậy và sự chính xác giả tạo nguy hiểm.

## 5.2 Các khái niệm đo lường cốt lõi

- **Độ đúng (Accuracy)**: Mức độ gần nhau giữa giá trị đo được và giá trị thực tế của đại lượng.
- **Độ chụm / Độ lặp lại (Precision / Repeatability)**: Mức độ trùng khớp giữa các kết quả của các phép đo lặp lại độc lập trong cùng điều kiện. Trong quan trắc địa kỹ thuật, **độ lặp lại quan trọng hơn độ đúng tuyệt đối**, vì mục tiêu hàng đầu là xác định **sự thay đổi tương đối ($\Delta$)** theo thời gian.
- **Độ phân giải (Resolution)**: Đại lượng biến thiên nhỏ nhất của thông số đo mà thiết bị có thể phân biệt và hiển thị được.
- **Độ trôi (Drift)**: Sự thay đổi số đọc theo thời gian không liên quan đến biến động thực tế của đại lượng cần đo (thường do lão hóa linh kiện điện tử, suy giảm từ tính hoặc ăn mòn kim loại).

## 5.3 Tính tương thích (Conformance)

Tính tương thích là khả năng của thiết bị hòa nhập vào môi trường đất đá mà không làm xáo trộn trường ứng suất, trường biến dạng hoặc mạng lưới đường dòng thấm xung quanh điểm đo:

- Một hộp đo áp lực đất nếu quá cứng so với đất xung quanh sẽ hút ứng suất về phía nó, dẫn đến số đọc cao hơn thực tế (over-registration).
- Một áp kế piezometer nếu có độ trễ thể tích quá lớn sẽ làm biến dạng trường áp lực nước lỗ rỗng cục bộ.

## 5.4 So sánh 4 nguyên lý cảm biến chính

| Họ cảm biến | Nguyên lý | Ưu điểm | Nhược điểm |
|---|---|---|---|
| **Cơ học (Mechanical)** | Thước kẹp, đồng hồ so (dial gauge), panme | Trực quan, giá rẻ, không cần nguồn điện | Chỉ đo được trên bề mặt lộ thiên, tốn nhân công |
| **Thủy lực (Hydraulic)** | Dầu hoặc nước truyền áp lực qua ống đến đồng hồ Bourdon | Độ bền cơ học cao, chịu môi trường ăn mòn | Độ trễ thời gian lớn, nhạy cảm với bọt khí và đóng băng |
| **Khí nén (Pneumatic)** | Màng cao su cân bằng áp lực khí | Không có linh kiện điện tử ngầm, miễn nhiễm sét | Tốc độ đo chậm, chỉ đo thủ công từng điểm |
| **Dây rung (Vibrating Wire - VW)** | Dây thép dao động từ tính theo tần số cộng hưởng | **Chuẩn vàng công nghiệp**: Tín hiệu tần số truyền xa không suy hao, độ bền > 20 năm | Cần thiết bị đọc chuyên dụng, cần hiệu chỉnh nhiệt độ |
| **Điện / MEMS (Electrical / MEMS)** | Cầu điện trở lá, vi cơ điện tử MEMS | Kích thước siêu nhỏ, xuất tín hiệu số trực tiếp (RS-485) | Nhạy cảm với sét lan truyền, cần kiểm soát độ trôi |

## 5.5 Hệ thống thu thập dữ liệu tự động (ADAS / ADAQS)

Dunnicliff khẳng định ADAS là cuộc cách mạng nâng cao tần suất và độ an toàn quan trắc, nhưng cần được thiết kế có dự phòng:

- **Datalogger tại chỗ**: Sử dụng vi điều khiển công suất thấp (Low-power microcontrollers) chạy bằng pin ắc quy nạp năng lượng mặt trời.
- **Truyền thông vô tuyến tầm xa**: Sử dụng công nghệ vô tuyến công suất thấp Sub-GHz / LoRa tạo mạng lưới mắt lưới (Mesh network) truyền dữ liệu về trạm Gateway trung tâm.
- **Nền tảng giám sát đám mây**: Tự động giải mã tín hiệu thô, tính toán giá trị kỹ thuật, vẽ đồ thị tiến độ và kích hoạt cảnh báo tự động qua SMS/Email khi chạm ngưỡng rủi ro.

## 5.6 Các điểm then chốt cần ghi nhớ

- Mọi phép đo đều có sai số; hiểu rõ độ không đảm bảo đo là bắt buộc để diễn giải đúng số liệu.
- Độ lặp lại (repeatability) là tiêu chí quan trọng nhất để theo dõi biến thiên theo thời gian.
- Công nghệ dây rung (VW) là tiêu chuẩn tin cậy hàng đầu cho các cảm biến chôn sâu dài hạn.
- Hệ thống tự động ADAS nâng cao năng lực quan trắc nhưng phải có giải pháp chống sét và nguồn dự phòng độc lập.
