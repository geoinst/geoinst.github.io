# Báo Cáo Kỹ Thuật: Tích Hợp Video Tư Liệu Quan Trắc & Học Thuật Địa Kỹ Thuật (YouTube Video Integration Report)

- **Dự án**: Geotechnical Instrumentation Knowledge Base (`geoinst.github.io`)
- **Phạm vi thực hiện**: Toàn bộ hệ thống Sổ tay tham khảo Tiếng Việt (`docs/vi/reference-manuals/`) và Tiếng Anh (`docs/reference-manuals/`)
- **Ngày thực hiện**: 13/10/2026
- **Trạng thái**: Hoàn thành & Đã xuất bản lên Production:
  - Bản tiếng Việt: [https://geoinst.github.io/vi/reference-manuals/](https://geoinst.github.io/vi/reference-manuals/)
  - Bản tiếng Anh: [https://geoinst.github.io/reference-manuals/](https://geoinst.github.io/reference-manuals/)

---

## 1. Mục Tiêu & Tiêu Chí Phân Tuyến Nguồn Tư Liệu (Source Taxonomy)

Nhằm nâng cao chất lượng học thuật và giá trị thực hành của kho tri thức địa kỹ thuật, dự án đã xây dựng quy chế phân cấp nguồn tư liệu video theo nguyên tắc:
1. **Nguồn công nghệ công nghiệp chính (Primary Industry Source)**: Kênh chính thức của tập đoàn **Orica Digital Solutions / GroundProbe** ([@orica/videos](https://www.youtube.com/@orica/videos)) — công nghệ giám sát radar mái dốc (SSR), giải pháp số hóa GeoSolutions, an toàn đập đuôi quặng (TSF) và kiểm soát rung chấn.
2. **Nguồn học thuật, viện nghiên cứu & trường đại học (Academic, Research Institutes & Universities)**: Khi tài liệu mang tính chất giáo trình kinh điển, lý thuyết nền tảng hoặc cơ sở thực nghiệm mà Orica không có video chuyên đề tương ứng, video được tuyển chọn từ các tổ chức học thuật uy tín hàng đầu thế giới (**hoàn toàn không sử dụng video từ các đối thủ cạnh tranh thương mại của Orica và RST Instruments**):
   - **ISSMGE** (Hội Cơ học Đất và Địa kỹ thuật Công trình Quốc tế)
   - **Geo-Institute of ASCE** (Viện Địa kỹ thuật - Hội Kỹ sư Xây dựng Hoa Kỳ): Chuỗi bài giảng danh dự Karl Terzaghi Lecture, Peck Lecture
   - **TS. Evert Hoek / Rocscience**: Chuỗi bài giảng kinh điển về Cơ học Đá (*Hoek's Corner*)
   - **ASDSO** (Hiệp hội Chuyên gia An toàn Đập Hoa Kỳ - hợp tác cùng FEMA & USSD)
   - **CGS** (Hội Địa kỹ thuật Canada — cơ quan biên soạn CFEM)
   - **IIT Roorkee / NPTEL** (Viện Công nghệ & Chương trình Giáo dục Công nghệ Quốc gia)
3. **Nguồn thực hành hiện trường thứ cấp (Secondary Practical Sources)**:
   - **RST Instruments** ([@RSTgeotechnical](https://www.youtube.com/@RSTgeotechnical/videos)) — hướng dẫn lắp đặt thiết bị, lấy số đọc cảm biến dây rung, inclinometer, piezometer, load cells.
   - **Measurand** ([@MeasurandVideos](https://www.youtube.com/@MeasurandVideos)) — giải pháp đo biến dạng sâu tự động hóa với mảng gia tốc kế ShapeArray (SAA, SAAV, SAAV Extend).
4. **Tiêu chuẩn nhúng giao diện**:
   - Tương thích chuẩn responsive 16:9 (`padding-bottom: 56.25%`, chiều rộng co giãn 100%, bo góc mềm mại `border-radius: 6px`).
   - Sử dụng domain tăng cường bảo mật `youtube-nocookie.com/embed/{id}`.

---

## 2. Tiêu Chuẩn Kỹ Thuật & Cấu Trúc Khung Nhúng (Embed Architecture)

### 2.1. Khung Nhúng Video Chính (Responsive 16:9 Container)
```html
<div class="video-container" style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; margin-bottom: 1rem;">
  <iframe src="https://www.youtube-nocookie.com/embed/{VIDEO_ID}" 
          title="{TIÊU_ĐỀ_VIDEO}" 
          frameborder="0" 
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
          allowfullscreen 
          style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border-radius: 6px;"></iframe>
</div>
<p><em>Featured Video: {Mô tả tóm tắt nội dung video & Nguồn cấp}.</em></p>
```

### 2.2. Khối Tư Liệu Thực Hành Thứ Cấp (Callout Admonition)
```markdown
!!! tip "Complementary Practical Field Resources from RST Instruments & Measurand (Terra Insights)"
    - **RST Instruments (@RSTgeotechnical):** [{Tên Video}](https://www.youtube.com/watch?v={ID}){ target="_blank" }  
      *{Mô tả quy trình lắp đặt, kiểm định hoặc vận hành thiết bị tại hiện trường}.*
    - **Measurand (@MeasurandVideos):** [{Tên Video}](https://www.youtube.com/watch?v={ID}){ target="_blank" }  
      *{Ứng dụng quan trắc tự động với ShapeArray SAA thay thế hoặc kết hợp đo thủ công}.*
```

---

## 3. Bảng Ma Trận Phân Bổ Video Cho Toàn Bộ 18 Tài Liệu Tham Khảo

| STT | Tài liệu tham khảo | Video chính & Nguồn phát | Phân loại nguồn | Video bổ trợ RST Instruments | Video bổ trợ Measurand |
|:---:|:---|:---|:---|:---|:---|
| **0** | **Mục lục tổng quan** (`index.md`) | `0tLX-O9dOQk` (Orica GeoSolutions GSS) | Orica Digital Solutions | `HJISt9or_Dw` (VW Piezometer) | `518Mx-65rI0` (ShapeArray Deflection) |
| **1** | **Tầm nhìn tổng thể & Khung tích hợp** (`overarching-vision.md`) | `0tLX-O9dOQk` (Orica GeoSolutions GSS) | Orica Digital Solutions | `dCjR64jX7B0` (Wireless Data Collection) | `_w6aW8yLq2Y` (Automated SAA System) |
| **2** | **John Dunnicliff — Sổ tay kinh điển** (`dunnicliff/index.md`) | `jKVrdiKbsoQ` (Orica GeoSolutions Platform) | Orica Digital Solutions | `HJISt9or_Dw` (Baseline VW Readings) | `518Mx-65rI0` (Real-time Deflection Monitoring) |
| **3** | **FHWA — Sổ tay quan trắc địa kỹ thuật** (`fhwa/index.md`) | `I6bdJXzuzlc` (GroundProbe SSR-XT / FX / Omni) | Orica / GroundProbe | `H2MVAVbOGdg` (Inclinometer Casing) | `idyme0c9HSs` (SAAV Extend Installation) |
| **4** | **FHWA — Tường chắn MSE & Mái dốc RSS** (`fhwa-mse-walls/index.md`) | `m0Xf9uycDns` (Fast Wall Starter) | Orica / GroundProbe | `H2MVAVbOGdg` (Inclinometer Casing) | `518Mx-65rI0` (Real-time Deflection) |
| **5** | **Kỹ thuật móng công trình** (`foundation-engineering/index.md`) | `bbcWWduZi9M` (Harry Poulos: Tall Building Foundations) | **Viện Địa kỹ thuật ASCE Geo-Institute** | `a5hHQaN1NkI` (Datalogger Wiring) | `YwQtxBBPS38` (SAAV Cyclical Install) |
| **6** | **Cơ học đất (Soil Mechanics)** (`soil-mechanics/index.md`) | `uElPkghqoJw` (What is Geotechnical Engineering?) | **Hội Địa kỹ thuật Quốc tế ISSMGE** | `HJISt9or_Dw` (Pore Water Pressure Readings) | `f3NMguxiZSE` (Rail Settlement SAA) |
| **7** | **Địa chất vật lý (Physical Geology)** (`physical-geology/index.md`) | `qGkkXNxnxAo` (Plate Tectonics & Crustal Dynamics) | **Viện Công nghệ IIT Roorkee / NPTEL** | `g3GAmDL5rrM` (RST Geotechnical) | `OtLkPOCQCoo` (SAAView 3D Analysis) |
| **8** | **GeoVadis Tập 1 — AI & Móng sâu** (`geovadis/index.md`) | `bNtg0iY5GwM` (AI FRAGTrack Analysis) | Orica Digital Solutions | `AQIWe60Meho` (RSTAR Dashboard) | `518Mx-65rI0` (Real-time ShapeArray) |
| **9** | **GeoVadis Tập 2 — Mái dốc & Hầm** (`geovadis-vol2/index.md`) | `I6bdJXzuzlc` (Next-gen SSR Slope Radars) | Orica / GroundProbe | `H2MVAVbOGdg` (Deep Inclinometer Casings) | `518Mx-65rI0` (ShapeArray for Tunnels & Slopes) |
| **10** | **GeoVadis Tập 3 — Nền móng & Mái dốc** (`geovadis-vol3/index.md`) | `0tLX-O9dOQk` (Orica GeoSolutions GSS) | Orica Digital Solutions | `BcghSAPrlKk` (RSTAR Wireless Webinar) | `idyme0c9HSs` (Modular SAAV Deployment) |
| **11** | **Giám sát hiệu năng đập (ASCE MOP-135)** (`monitoring-dam-performance/index.md`) | `lIvGH5bux5Q` (Dam Inspections & Safety) | **Hiệp hội An toàn Đập ASDSO / USSD** | `HJISt9or_Dw` (Dam Core Piezometers) | `518Mx-65rI0` (Automated Crest SAA) |
| **12** | **An toàn đập chất thải (ICOLD Bulletin 194)** (`tailings-dam-safety/index.md`) | `8yqLRjzVuvk` (Tailings Dam Monitoring Solution) | Orica / GroundProbe | `AQIWe60Meho` (RSTAR Dashboard) | `518Mx-65rI0` (Real-time Deflection) |
| **13** | **Cơ học đá thực hành Evert Hoek** (`practical-rock-engineering/index.md`) | `r0ezG4SmaXM` (Development of Rock Engineering) | **TS. Evert Hoek / Rocscience** | `H6FRo2VKeCs` (DT2485 Bus Logger) | `YwQtxBBPS38` (SAAV Cyclical Install) |
| **14** | **Sổ tay địa kỹ thuật Canada (CFEM)** (`cfem/index.md`) | `TA6BU4DD684` (Permafrost Geotechnical Engineering) | **Hội Địa kỹ thuật Canada CGS** | `BcghSAPrlKk` (RSTAR Wireless Webinar) | `518Mx-65rI0` (Cold Climate SAA) |
| **15** | **Cẩm nang Kỹ sư Địa kỹ thuật** (`geotechnical-engineers-handbook/index.md`) | `0tLX-O9dOQk` (Orica Geotech Services) | Orica Digital Solutions | `H2MVAVbOGdg` (Inclinometer Casing) | `idyme0c9HSs` (SAAV Installation) |
| **16** | **SME Mining Engineering Handbook** (`sme-mine-handbook/index.md`) | `I6bdJXzuzlc` (GroundProbe SSR) | Orica / GroundProbe | `xFplwoCngEU` (Wireless Data Collection) | `518Mx-65rI0` (Real-time Deflection) |
| **17** | **Cẩm nang Burt Look** (`burt-look-handbook/index.md`) | `TBHAw7g04W0` (Paul Mayne: Terzaghi Lecture on CPT) | **Viện Địa kỹ thuật ASCE Geo-Institute** | `s4ft0x6aPoc` (Field Utility App) | `OtLkPOCQCoo` (SAAView 3D Analysis) |

---

## 4. Quá Trình Triển Khai & Kiểm Định Kỹ Thuật

### 4.1. Tự Động Hóa Qua Git REST API
Toàn bộ quá trình đóng gói và xuất bản được thực hiện tự động hóa bằng Python và GitHub REST API:
1. Đọc nội dung tệp nguồn dưới dạng nhị phân UTF-8 thuần túy (`utf-8`), mã hóa Base64 và tạo Git Blob SHAs trên repository `geoinst/geoinst.github.io`.
2. Tạo Git Tree mới liên kết với commit cha gần nhất.
3. Tạo Git Commit mới có chữ ký tác giả (`geoinst <hpbcca@gmail.com>`).
4. Cập nhật con trỏ `refs/heads/main`.

### 4.2. Giám Sát CI/CD GitHub Actions & Kiểm Định Production
- **Workflow**: `Deploy MkDocs site to GitHub Pages` (.github/workflows/deploy.yml)
- **Kiểm định**: Tất cả các trang tiếng Anh và tiếng Việt được kiểm tra tải về trực tiếp, xác nhận hiển thị chính xác tiêu đề video học thuật, không có lỗi font và các liên kết hoạt động ổn định.
