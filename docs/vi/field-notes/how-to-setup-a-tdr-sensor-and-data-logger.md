---
title: Cách thiết lập một cảm biến TDR và bộ ghi dữ liệu TDR logger
category: BỘ GHI DỮ LIỆU
modified: Mon, 11 Jul, 2022 at 10:14 AM
article_id: 63000273146
lang: vi
lang_alt: field-notes/how-to-setup-a-tdr-sensor-and-data-logger/
---

# Cách thiết lập một cảm biến TDR và bộ ghi dữ liệu TDR logger


Nhấn và kéo "Coaxial" (Đồng trục) trong menu chọn đầu dò. Nếu sử dụng bộ ghép kênh (multiplexer), hãy chọn Multiplexer phù hợp. Gán tên cho mỗi cáp TDR. Đặt Vp thành 0,88 (Vận tốc truyền sóng - Velocity of Propagation). Số lần trung bình (Averages) được đặt là 4. Số điểm (Points) được đặt là 2000 để tạo 2000 điểm đo dọc theo chiều dài cáp. 'Cable Length' (Chiều dài cáp) là chiều dài đoạn cáp phía trên bề mặt đất. 'Window Length' (Chiều dài cửa sổ) là chiều dài đoạn cáp được lắp đặt trong lỗ khoan.

Sau khi thực hiện một phép đo, chọn Measure | Set Probe Baseline (Đo | Đặt đường cơ sở đầu dò) nếu bạn muốn sử dụng phép đo/dạng sóng hiện tại làm đường cơ sở (baseline). Dạng sóng cơ sở sẽ vẫn hiển thị trên đồ thị khi các phép đo bổ sung được thực hiện và hiển thị. (Lưu ý: để xem được phép đo cơ sở, bạn phải chọn View | Show Baseline measurement (Xem | Hiện phép đo cơ sở). Khi được chọn, sẽ có dấu tick bên cạnh mục đó trong menu.)

Trong ảnh chụp màn hình bên dưới, đường màu xanh lam mảnh thể hiện phép đo cơ sở; đường màu xanh lam đậm hơn thể hiện phép đo hiện tại.

Để biết thêm thông tin về cách sử dụng phần mềm, chọn PC-TDR Help (Trợ giúp PC-TDR) trong menu Help (Trợ giúp) ở thanh menu trên cùng.

Kết nối cáp đồng trục với cổng đồng trục trên bộ ghi dữ liệu TDR logger.

Kết nối cáp micro USB sang USB với thiết bị TDR 200 và máy tính.

Khởi động phần mềm PC-TDR và trên tab Network (Mạng) ở trang chính, chọn cổng nối tiếp (serial port) của máy tính mà bạn sẽ dùng để kết nối với bộ ghi dữ liệu TDR logger. Trong phần 'Selected Device Properties' (Thuộc tính thiết bị đã chọn). Nếu cần, trình điều khiển (driver) có thể được cài đặt, nhưng thông thường nó đã được cài đặt khi phần mềm PC-TDR được cài trên máy tính. Cổng nối tiếp được chọn bằng cách nhấp … và dùng menu thả xuống để chọn cổng USB mà bộ ghi dữ liệu TDR logger kết nối với máy tính. Các cài đặt khác không cần thay đổi.

Gán tên cho mỗi cáp TDR.

Đặt Vp thành 0,88 (Vận tốc truyền sóng).

Số lần trung bình (Averages) được đặt là 4

Số điểm (Points) được đặt là 2000 để tạo 2000 điểm đo dọc theo chiều dài cáp.

'Cable Length' (Chiều dài cáp) là chiều dài đoạn cáp phía trên bề mặt đất.

'Window Length' (Chiều dài cửa sổ) là chiều dài đoạn cáp được lắp đặt trong lỗ khoan.

Nhấn vào 'Graph' (Đồ thị) để xem đồ thị của 2000 điểm đo dọc theo chiều dài cáp được chôn trong lỗ khoan. Các giá trị sẽ dao động từ 0 đến 1, với đầu mút cáp dịch chuyển về giá trị 1.

Để thực hiện phép đo cáp đồng trục, nhấn nút làm mới (refresh) trên thanh công cụ hoặc chọn Measure | Refresh (Đo | Làm mới) từ menu. Các phép đo sẽ được hiển thị trong tab Graph (Đồ thị).

Xuất dữ liệu (Exporting Data) - Trong menu File, chọn 'Import Probe Data' (Nhập dữ liệu đầu dò) và làm theo hướng dẫn.

Lưu dữ liệu (Saving the data) - Chọn thư mục để lưu dữ liệu.

0.88

Measure | Refresh

Graph

Measure | Set Probe Baseline

View | Show Baseline
