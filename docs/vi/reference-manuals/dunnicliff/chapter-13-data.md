---
lang: vi
lang_alt: reference-manuals/dunnicliff/chapter-13-data/
---

# Chương 13 — Thu thập, xử lý, trình bày và diễn giải dữ liệu

## 13.1 Dữ liệu chỉ có giá trị khi được sử dụng

Những chồng sổ ghi chép dày cộp nằm phủ bụi trên giá sách không phải là quan trắc. Quan trắc thực sự là một quá trình liên tục biến đổi **những số đọc thô (raw readings)** thành **thông tin kỹ thuật có ý nghĩa** để chỉ huy trưởng và kỹ sư thiết kế đưa ra các quyết định hành động kịp thời trên công trường.

## 13.2 Số đọc ban đầu và đường cơ sở (Baseline Readings)

- **Thời điểm xác định**: Số đọc ban đầu (zero reading) phải được đo đạc sau khi quá trình đông cứng của vữa chèn đã ổn định hoàn toàn và trước khi bất kỳ tải trọng thi công nào (đào đất, hạ mực nước, chất tải đắp) bắt đầu tác động lên khu vực.
- **Quy trình đo lặp lại**: Bắt buộc phải thực hiện tối thiểu **3 chu kỳ đo độc lập** tại các thời điểm nhiệt độ khác nhau trong ngày để tính giá trị trung bình chuẩn và xác nhận độ lặp lại của cảm biến. Mọi biến thiên sau này đều được so sánh tương đối với số đọc đường cơ sở này.

## 13.3 Tần suất quan trắc (Monitoring Frequency)

Tần suất đo không phải là một con số cố định mà phải thay đổi linh hoạt theo mức độ rủi ro và tốc độ thi công:
- **Giai đoạn thi công tích cực (đào hố sâu, đắp tải nhanh, khoan kích hầm)**: Đo hàng ngày, hoặc đo liên tục 15–30 phút/lần bằng hệ thống tự động ADAS.
- **Giai đoạn tạm dừng hoặc sau khi thi công xong**: Đo 1–2 lần/tuần.
- **Giai đoạn vận hành dài hạn**: Đo 1–2 lần/tháng, và tăng cường đo ngay sau các sự kiện đặc biệt (mưa bão lớn, động đất, tích nước hồ chứa).

## 13.4 Kiểm tra tính hợp lý của số liệu (Data Validation)

Trước khi nhập số liệu vào báo cáo, người kỹ sư phải tự đặt ra các câu hỏi phản biện:
- Số đọc có phản ánh đúng logic vật lý không? (Ví dụ: khi trời mưa lớn, áp lực nước lỗ rỗng phải tăng chứ không thể giảm vô lý).
- Sự thay đổi đột ngột là do hiện tượng địa kỹ thuật thực tế hay do lỗi thiết bị? (Cảm biến hỏng thường nhảy vọt tức thời hoặc mất tín hiệu; biến dạng địa chất thường phát triển tiệm tiến có xu hướng).
- Các thiết bị lân cận có ghi nhận phản ứng tương đồng không? (Đối chiếu chéo giữa Piezometer và Inclinometer trong cùng một mặt cắt).

## 13.5 Trình bày dữ liệu đồ thị trực quan

Dunnicliff yêu cầu biểu đồ quan trắc phải được vẽ song song trên cùng một trục hoành thời gian (chronological correlation plots) với:
1. **Tiến độ thi công thực tế**: Cao độ đáy hố đào, chiều cao khối đất đắp, tiến độ nổ mìn kích hầm.
2. **Yếu tố thời tiết tự nhiên**: Biểu đồ cột lượng mưa hàng ngày và nhiệt độ không khí.
3. **Mực nước ngầm tự nhiên**: Theo dõi từ các giếng quan trắc đối chứng ngoài phạm vi thi công.
4. **Các đường ngưỡng hành động**: Thể hiện rõ các đường giới hạn Cảnh báo (Alert limit) và Báo động (Action limit).

## 13.6 Diễn giải dữ liệu và lập báo cáo kỹ thuật

Mọi báo cáo quan trắc gửi cho Chủ đầu tư và Tư vấn giám sát bắt buộc phải có phần **Đánh giá và Diễn giải kỹ thuật của Chuyên gia (Engineering Assessment)**:
- Tóm tắt các diễn biến chính trong kỳ báo cáo.
- So sánh biến dạng thực tế với các giá trị dự báo trong thuyết minh thiết kế.
- Kết luận rõ ràng: Công trình đang ở trạng thái **Bình thường (Normal)**, **Cần theo dõi sát (Attention)** hay **Nguy hiểm (Alarm)**, đi kèm khuyến nghị giải pháp xử lý cụ thể.

![Figure: dunnicliff-data-timeline](../../../assets/figures/dunnicliff-data-timeline.svg)

**Hình.** Từ đường cơ sở đến vận hành. Đánh giá thay đổi so với đường cơ sở và vẽ số đọc theo biến số dẫn động (Dunnicliff, Ch. 18).

## 13.7 Các điểm then chốt cần ghi nhớ

- Số đọc ban đầu (baseline) phải được đo lặp lại tối thiểu 3 lần trong điều kiện ổn định.
- Tần suất đo phải tỷ lệ thuận với tốc độ thi công và mức độ rủi ro công trình.
- Luôn kiểm tra tính hợp lý và đối chiếu chéo giữa các họ cảm biến khác nhau.
- Vẽ biểu đồ quan trắc tương quan trực tiếp với tiến độ đào đắp và lượng mưa.
- Báo cáo phải có phần đánh giá kỹ thuật và đề xuất hành động rõ ràng.
