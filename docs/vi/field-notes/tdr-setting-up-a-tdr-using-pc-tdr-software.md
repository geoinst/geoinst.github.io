---
title: Bộ ghi dữ liệu TDR – Thiết lập TDR bằng phần mềm PC-TDR
category: BỘ GHI DỮ LIỆU
modified: Tue, 20 Aug, 2024 at  1:33 PM
article_id: 63000283904
lang: vi
lang_alt: field-notes/tdr-setting-up-a-tdr-using-pc-tdr-software/
---

# Bộ ghi dữ liệu TDR – Thiết lập TDR bằng phần mềm PC-TDR

Khi sử dụng phần mềm PC-TDR để kết nối với TDR qua giao diện bộ ghi dữ liệu TDR logger. Khởi động phần mềm và kết nối bộ ghi dữ liệu TDR logger bằng cáp Micro-USB với cổng USB trên máy tính. Trong menu View (Xem), chọn Set Default Layout (Đặt bố cục mặc định) để sử dụng toàn màn hình.

Để thêm một cấu hình mới và TDR, từ menu thả xuống phía trên, nhấn New (Mới).

Nhấn vào ô bộ ghi dữ liệu TDR logger để đặt cổng com (com port) mà TDR sẽ kết nối qua. Người vận hành sẽ được yêu cầu chọn cổng com và cài đặt trình điều khiển.

Khi bộ ghi dữ liệu TDR logger được kết nối với máy tính bằng cáp giao tiếp micro-USB, thiết bị sẽ được cấp nguồn và kết nối. Hãy kiểm tra các cổng com trong 'Device Manager' (Trình quản lý thiết bị) để xác định cổng mà TDR kết nối vào. Bộ ghi dữ liệu TDR logger sẽ hiển thị dưới tên TDR logger trong trình quản lý thiết bị, nhưng có thể không được nhận diện tương ứng trong các tùy chọn cổng com của phần mềm PC-TDR. Trong ví dụ bên dưới, cổng được nhận diện là bộ ghi dữ liệu dòng DT, nhưng điều quan trọng là số cổng. Nếu bộ ghi dữ liệu TDR logger không xuất hiện trong trình quản lý thiết bị, thì các trình điều khiển chưa được cài đặt đúng cách.

Trong mục Ports (Cổng), bộ ghi dữ liệu TDR logger được kết nối với cổng 29.

Địa chỉ SDM chỉ được thay đổi khi nhiều bộ ghép kênh SDMX850 hoặc SDMX50 được sử dụng khi kết nối với một bộ ghi dữ liệu duy nhất.

Khi thêm thiết bị, sử dụng nút màu xanh lá + và chọn 'Coaxial' (Đồng trục).

Sau khi TDR đã được cấu hình, hãy gán một Tên đầu dò (Probe Name). Tất cả các TDR nên được cấu hình bằng các giá trị được liệt kê bên dưới.

Lưu TDR sau khi thiết lập với cùng tên đầu dò.

Sau khi các thuộc tính TDR được đặt, hãy đánh dấu chọn và tích vào ô kiểm (check box) ở phía bên trái màn hình cho TDR, sau đó nhấn nút làm mới (refresh).

Đồ thị sẽ được hiển thị, và thanh bên trái sẽ hiện thông báo đo thành công (measurement succeeded).

Khi lưu các tệp dữ liệu, ảnh chụp màn hình đồ thị nên được lưu và dữ liệu có thể được lưu bằng cách Xuất dữ liệu (Exporting the data).

Xuất các giá trị đo (Export Readings) với tùy chọn 'append selected' (thêm vào các mục đã chọn).

Vp = 0.88;

Averages = 4;

Points = 2000;

Cable length = the length of cable above the surface of the borehole to the data logger;

Window Length = Length of cable grouted in the borehole.

Probe Length = 0.3;

Probe Offset = 0;

Probe Kp = 0.

[Image: A screenshot of a computer

Description automatically generated]

[Image: A screenshot of a computer

Description automatically generated]

[Image: A screenshot of a computer error

Description automatically generated]

[Image: A screenshot of a computer error

Description automatically generated]

[Image: A screenshot of a computer

Description automatically generated]

[Image: A white background with black and white clouds

Description automatically generated]

[Image: A screenshot of a computer

Description automatically generated]

[Image: A screenshot of a computer

Description automatically generated]

[Image: A screen shot of a computer

Description automatically generated]
