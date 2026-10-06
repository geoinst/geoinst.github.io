---
lang: vi
lang_alt: reference-manuals/dunnicliff/chapter-03-planning/
---

# Chương 3 — Tiếp cận có hệ thống để lập kế hoạch chương trình quan trắc

## 3.1 Trọng tâm cốt lõi của ngành quan trắc

Nếu cuốn cẩm nang của Dunnicliff chỉ được phép giữ lại một chương duy nhất, thì đó chính là chương này. Một chương trình quan trắc được lập kế hoạch có hệ thống — thay vì làm theo thói quen máy móc hay sao chép sơ đồ bố trí của một dự án khác — sẽ đem lại dữ liệu thực sự hữu ích, tin cậy và có giá trị pháp lý cao.

## 3.2 Đặt ra các câu hỏi địa kỹ thuật trước tiên

Trước khi quyết định chọn mua bất kỳ cảm biến nào, kỹ sư phải liệt kê rõ ràng các câu hỏi địa kỹ thuật cụ thể mà chương trình cần trả lời:

- Liệu chuyển vị ngang của tường vây hố đào sâu có vượt quá giới hạn 25 mm cho phép hay không?
- Áp lực nước lỗ rỗng thặng dư dưới khối đắp có đang tiêu tán đủ nhanh để cho phép đắp phân tầng tiếp theo không?
- Mái dốc tự nhiên có đang hình thành cung trượt sâu sau các đợt mưa lớn không?
- Vòm hầm có bị võng hoặc hội tụ ngang vượt ngưỡng thiết kế trong quá trình đào không?

Mỗi câu hỏi kỹ thuật sẽ trực tiếp chỉ ra **thông số cần đo**, **vị trí lắp đặt** và **quyết định hành động tương ứng**.

## 3.3 Quy trình lập kế hoạch 20 bước của Dunnicliff

Một kế hoạch hoàn chỉnh phải tuân thủ nghiêm ngặt 20 bước tuần tự:

1. **Xác định điều kiện dự án**: Hình học công trình, địa tầng, mực nước ngầm, phương pháp thi công.
2. **Nhận diện cơ chế địa kỹ thuật**: Các hình thức mất ổn định hoặc biến dạng có thể xảy ra.
3. **Xác định các câu hỏi địa kỹ thuật cụ thể**: Trọng tâm định hướng toàn bộ chương trình.
4. **Xác định mục đích dữ liệu**: Kiểm tra thiết kế, an toàn thi công hay vận hành lâu dài.
5. **Lựa chọn thông số cần đo**: Áp lực nước, chuyển vị ngang, độ lún đứng, ứng suất, lực tải.
6. **Dự đoán dải biến thiên**: Ước tính phạm vi giá trị tối đa và tối thiểu để chọn dải đo cảm biến phù hợp.
7. **Thiết lập ngưỡng hành động (Alert / Alarm / Action)**: Phân định mức cảnh báo xanh, vàng, đỏ.
8. **Lựa chọn loại thiết bị**: Đánh giá nguyên lý cảm biến, độ tin cậy và khả năng sống sót trong môi trường công trường.
9. **Xác định vị trí, độ sâu và số lượng thiết bị**: Bố trí tại các mặt cắt đặc trưng và các vị trí xung yếu nhất.
10. **Lập kế hoạch thu thập dữ liệu**: Tần suất đo, phương thức đo thủ công hay tự động hóa ADAS.
11. **Xác định ngân sách sai số & độ chính xác**: Độ phân giải, độ lặp lại và các hiệu chỉnh cần thiết.
12. **Dự trù tác động môi trường**: Nhiệt độ khắc nghiệt, chống sét lan truyền, chống ẩm và chống phá hoại.
13. **Chuẩn bị quy trình lắp đặt chi tiết**: Phương pháp khoan, dung dịch khoan, tỷ lệ vữa chèn, bảo vệ miệng lỗ.
14. **Kế hoạch xử lý và diễn giải số liệu**: Phần mềm quản lý dữ liệu, kiểm tra tính hợp lý, biểu đồ trực quan.
15. **Phân định trách nhiệm nhân sự**: Ai là người đọc, ai kiểm tra, ai phân tích, ai ra quyết định.
16. **Lập dự toán chi phí toàn diện**: Bao gồm mua sắm, lắp đặt, bảo trì, vận hành và phân tích số liệu.
17. **Soạn thảo hồ sơ thông số kỹ thuật (Specs)**: Rõ ràng, chặt chẽ và có chế tài nghiệm thu.
18. **Lựa chọn hình thức hợp đồng**: Tránh đấu thầu giá thấp nhất; ưu tiên đánh giá năng lực kỹ thuật.
19. **Kế hoạch bảo trì và bảo vệ thiết bị**: Bảo vệ cơ học, thay hạt hút ẩm, kiểm tra định kỳ.
20. **Kế hoạch nghiệm thu và kết thúc (Decommissioning)**: Bàn giao hoặc lấp hủy an toàn khi kết thúc dự án.

## 3.4 Tiêu chí lựa chọn thiết bị

Việc chọn thiết bị phải cân bằng giữa các yếu tố:

- **Tính phù hợp (Suitability)**: Phù hợp với môi trường địa chất và đại lượng cần đo.
- **Độ chính xác và dải đo**: Độ chính xác phải đủ để phục vụ quyết định kỹ thuật, không lãng phí chi phí cho độ chính xác thừa.
- **Độ bền và khả năng sống sót (Durability)**: Khả năng chống nước ngập (IP68), chịu rung chấn thi công.
- **Nguồn điện và truyền dữ liệu**: Pin năng lượng mặt trời, truyền thông vô tuyến tầm xa.

## 3.5 Dự toán ngân sách và phân kỳ đầu tư

Quan trắc sẽ tiết kiệm chi phí nhất khi được đưa vào thiết kế ngay từ đầu dự án. Dự toán phải bao quát toàn bộ vòng đời: mua sắm thiết bị chỉ chiếm khoảng 30-40% tổng chi phí; phần còn lại dành cho lắp đặt chuyên nghiệp, bảo trì và phân tích dữ liệu chuyên gia.

!!! warning "Sai lầm phổ biến nhất trong lập kế hoạch"
    Lắp đặt thiết bị chỉ để "cho có số liệu" mà không hề có câu hỏi kỹ thuật định hướng, không có kế hoạch đọc số liệu định kỳ và không có phương án hành động khi số liệu vượt ngưỡng. Những thiết bị như vậy chỉ là đồ trang trí lãng phí.

## 3.6 Các điểm then chốt cần ghi nhớ

- Luôn lập kế hoạch có hệ thống; xác định rõ câu hỏi kỹ thuật trước khi chọn mua thiết bị.
- Mỗi câu hỏi kỹ thuật quyết định trực tiếp thông số đo, vị trí đặt và phương án xử lý.
- Cân bằng giữa tính phù hợp, độ bền, độ chính xác và chi phí đầu tư.
- Lập dự toán cho toàn bộ vòng đời của hệ thống quan trắc, không chỉ riêng chi phí mua thiết bị.
