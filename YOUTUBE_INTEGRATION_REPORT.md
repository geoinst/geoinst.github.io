# Báo Cáo Kỹ Thuật: Tích Hợp Video Tư Liệu Quan Trắc Địa Kỹ Thuật (YouTube Video Integration Report)

- **Dự án**: Geotechnical Instrumentation Knowledge Base (`geoinst.github.io`)
- **Phạm vi thực hiện**: Toàn bộ hệ thống Sổ tay tham khảo Tiếng Việt (`docs/vi/reference-manuals/`) và Tiếng Anh (`docs/reference-manuals/`)
- **Ngày thực hiện**: 13/10/2026
- **Trạng thái**: Hoàn thành & Đã xuất bản lên Production:
  - Bản tiếng Việt: [https://geoinst.github.io/vi/reference-manuals/](https://geoinst.github.io/vi/reference-manuals/)
  - Bản tiếng Anh: [https://geoinst.github.io/reference-manuals/](https://geoinst.github.io/reference-manuals/)

---

## 1. Mục Tiêu & Yêu Cầu Dự Án

Nhằm nâng cao chất lượng trực quan và giá trị thực hành của kho tri thức địa kỹ thuật, dự án đã tiến hành rà soát, lựa chọn và nhúng các video kỹ thuật thực địa vào từng tài liệu tham khảo trên cả hai phiên bản ngôn ngữ:
1. **Nguồn video chính (Primary Source)**: Kênh chính thức của tập đoàn **Orica Digital Solutions / GroundProbe** ([@orica/videos](https://www.youtube.com/@orica/videos)) — công nghệ giám sát radar mái dốc, chuyển động ngầm, quản lý an toàn đập đuôi quặng và dịch vụ chuyên gia GSS.
2. **Nguồn video thứ cấp & bổ trợ (Secondary Sources)**:
   - **RST Instruments** ([@RSTgeotechnical](https://www.youtube.com/@RSTgeotechnical/videos)) — hướng dẫn lắp đặt thiết bị, lấy số đọc cảm biến dây rung, inclinometer, piezometer, load cells.
   - **Measurand** ([@MeasurandVideos](https://www.youtube.com/@MeasurandVideos)) — giải pháp đo biến dạng sâu tự động hóa với mảng gia tốc kế ShapeArray (SAA, SAAV, SAAV Extend).
3. **Tiêu chuẩn nhúng giao diện**:
   - Tương thích chuẩn responsive 16:9 (`padding-bottom: 56.25%`, chiều rộng co giãn 100%, bo góc mềm mại `border-radius: 6px`).
   - Kế thừa phong cách bố cục chuẩn từ dự án tri thức thể thao New Tennis Knowledge ([tham khảo mẫu](https://tennis-unified.github.io/en/articles/EN-tenniskb-ground-reaction-forces-grf-vertical-vs-horizontal-vectors/)).
   - Sử dụng domain tăng cường bảo mật `youtube-nocookie.com/embed/{id}`.
4. **Triển khai & Phát hành**: Tự động hóa cập nhật và triển khai thông qua GitHub Personal Access Token (PAT) và GitHub Actions.

---

## 2. Tiêu Chuẩn Kỹ Thuật & Cấu Trúc Khung Nhúng (Embed Architecture)

### 2.1. Khung Nhúng Video Chính (Responsive 16:9 Container)
Mỗi tài liệu được tích hợp một khung player HTML responsive:

```html
<div class="video-container" style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; margin-bottom: 1rem;">
  <iframe src="https://www.youtube-nocookie.com/embed/{VIDEO_ID}" 
          title="{TIÊU_ĐỀ_VIDEO}" 
          frameborder="0" 
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
          allowfullscreen 
          style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border-radius: 6px;"></iframe>
</div>
<p><em>Featured Video (Primary Source — Orica): {Mô tả tóm tắt nội dung video}.</em></p>
```

### 2.2. Khối Tư Liệu Thực Hành Thứ Cấp (Callout Admonition)
Sử dụng cú pháp Material for MkDocs (`!!! tip`) kết hợp icon YouTube và button điều hướng:

```markdown
!!! tip "Complementary Practical Field Resources from RST Instruments & Measurand (Terra Insights)"
    - **RST Instruments (@RSTgeotechnical):** [{Tên Video}](https://www.youtube.com/watch?v={ID}){ target="_blank" }  
      *{Mô tả quy trình lắp đặt, kiểm định hoặc vận hành thiết bị tại hiện trường}.*
    - **Measurand (@MeasurandVideos):** [{Tên Video}](https://www.youtube.com/watch?v={ID}){ target="_blank" }  
      *{Ứng dụng quan trắc tự động với ShapeArray SAA thay thế hoặc kết hợp đo thủ công}.*
```

---

## 3. Bảng Ma Trận Phân Bổ Video Cho Tài Liệu Tham Khảo (Cả 2 Bản Ngôn Ngữ)

| STT | Tài liệu tham khảo (VI / EN) | Video chính (Orica / GroundProbe) | Video bổ trợ RST Instruments | Video bổ trợ Measurand |
|:---:|:---|:---|:---|:---|
| **0** | **Mục lục tổng quan** (`reference-manuals/index.md`) | `0tLX-O9dOQk` (Geosolutions GSS) | `HJISt9or_Dw` (VW Piezometer) | `518Mx-65rI0` (ShapeArray Deflection) |
| **1** | **Tầm nhìn tổng thể & Khung tích hợp** (`overarching-vision.md`) | `0tLX-O9dOQk` (Geosolutions GSS) | `dCjR64jX7B0` (Wireless Data Collection) | `_w6aW8yLq2Y` (Automated SAA System) |
| **2** | **John Dunnicliff — Sổ tay kinh điển** (`dunnicliff/index.md`) | `jKVrdiKbsoQ` (Digital Solutions GeoSolutions) | `HJISt9or_Dw` (Baseline VW Readings) | `518Mx-65rI0` (Real-time Deflection Monitoring) |
| **3** | **FHWA — Sổ tay quan trắc địa kỹ thuật** (`fhwa/index.md`) | `I6bdJXzuzlc` (GroundProbe SSR-XT / FX / Omni) | `H2MVAVbOGdg` (Inclinometer Casing Installation) | `idyme0c9HSs` (SAAV Extend Installation) |
| **4** | **FHWA — Tường chắn MSE & Mái dốc RSS** (`fhwa-mse-walls/index.md`) | `m0Xf9uycDns` (Fast Wall Starter) | `H2MVAVbOGdg` (Inclinometer Casing) | `518Mx-65rI0` (Real-time Deflection) |
| **5** | **Kỹ thuật móng công trình** (`foundation-engineering/index.md`) | `0tLX-O9dOQk` (Orica GeoSolutions GSS) | `a5hHQaN1NkI` (Datalogger Wiring) | `YwQtxBBPS38` (SAAV Cyclical Install) |
| **6** | **Cơ học đất (Soil Mechanics)** (`soil-mechanics/index.md`) | `gl7yck1xbog` (GroundProbe GNSS System) | `HJISt9or_Dw` (Pore Water Pressure Readings) | `f3NMguxiZSE` (Rail Settlement SAA) |
| **7** | **Địa chất vật lý (Physical Geology)** (`physical-geology/index.md`) | `I6bdJXzuzlc` (GroundProbe Slope Radar) | `g3GAmDL5rrM` (RST Geotechnical) | `OtLkPOCQCoo` (SAAView 3D Analysis) |
| **8** | **GeoVadis Tập 1 — AI & Móng sâu** (`geovadis/index.md`) | `bNtg0iY5GwM` (AI FRAGTrack Analysis) | `AQIWe60Meho` (RSTAR Dashboard) | `518Mx-65rI0` (Real-time ShapeArray) |
| **9** | **GeoVadis Tập 2 — Ổn định mái dốc & Hầm** (`geovadis-vol2/index.md`) | `I6bdJXzuzlc` (Next-gen SSR Slope Radars) | `H2MVAVbOGdg` (Deep Inclinometer Casings) | `518Mx-65rI0` (ShapeArray for Tunnels & Slopes) |
| **10** | **GeoVadis Tập 3 — Nền móng & Mái dốc** (`geovadis-vol3/index.md`) | `0tLX-O9dOQk` (Orica GeoSolutions GSS) | `BcghSAPrlKk` (RSTAR Wireless Webinar) | `idyme0c9HSs` (Modular SAAV Deployment) |
| **11** | **Giám sát hiệu năng đập (ASCE MOP-135)** (`monitoring-dam-performance/index.md`) | `I6bdJXzuzlc` (GroundProbe SSR) | `HJISt9or_Dw` (Dam Core Piezometers) | `518Mx-65rI0` (Automated Crest SAA) |
| **12** | **An toàn đập chất thải (ICOLD Bulletin 194)** (`tailings-dam-safety/index.md`) | `8yqLRjzVuvk` (Tailings Dam Monitoring Solution) | `AQIWe60Meho` (RSTAR Dashboard) | `518Mx-65rI0` (Real-time Deflection) |
| **13** | **Cơ học đá thực hành Evert Hoek** (`practical-rock-engineering/index.md`) | `F16e2U7MRGc` (Tunnel Blast Vibration) | `H6FRo2VKeCs` (DT2485 Bus Logger) | `YwQtxBBPS38` (SAAV Cyclical Install) |
| **14** | **Sổ tay địa kỹ thuật Canada (CFEM)** (`cfem/index.md`) | `0tLX-O9dOQk` (Orica GeoSolutions GSS) | `BcghSAPrlKk` (RSTAR Wireless Webinar) | `518Mx-65rI0` (Cold Climate SAA) |
| **15** | **Cẩm nang Kỹ sư Địa kỹ thuật** (`geotechnical-engineers-handbook/index.md`) | `0tLX-O9dOQk` (Orica Geotech Services) | `H2MVAVbOGdg` (Inclinometer Casing) | `idyme0c9HSs` (SAAV Installation) |
| **16** | **SME Mining Engineering Handbook** (`sme-mine-handbook/index.md`) | `I6bdJXzuzlc` (GroundProbe SSR) | `xFplwoCngEU` (Wireless Data Collection) | `518Mx-65rI0` (Real-time Deflection) |
| **17** | **Cẩm nang Burt Look** (`burt-look-handbook/index.md`) | `gl7yck1xbog` (GroundProbe GNSS System) | `s4ft0x6aPoc` (Field Utility App) | `OtLkPOCQCoo` (SAAView 3D Analysis) |

---

## 4. Quá Trình Triển Khai & Kiểm Định Kỹ Thuật

### 4.1. Tự Động Hóa Qua Git REST API
Toàn bộ quá trình đóng gói và xuất bản được thực hiện tự động hóa bằng PowerShell và GitHub REST API:
1. Đóng gói các tệp nguồn Markdown dưới dạng Base64 và tạo Git Blob SHAs trên repository `geoinst/geoinst.github.io`.
2. Tạo Git Tree mới liên kết với commit cha gần nhất.
3. Tạo Git Commit mới có chữ ký tác giả (`geoinst <hpbcca@gmail.com>`).
4. Cập nhật con trỏ `refs/heads/main`.

### 4.2. Giám Sát CI/CD GitHub Actions
- **Workflow**: `Deploy MkDocs site to GitHub Pages` (.github/workflows/deploy.yml)
- **Kiểm định**: Tất cả các trang tiếng Anh và tiếng Việt được biên dịch tĩnh và triển khai đồng bộ lên GitHub Pages.

---

## 5. Hướng Dẫn Bảo Trì & Mở Rộng

1. **Thêm video mới**: Khi có sản phẩm hoặc tài liệu mới, sao chép khối `video-container` và thay thế ID YouTube tương ứng.
2. **Kiểm tra liên kết định kỳ**: Các liên kết từ YouTube channels (@orica, @RSTgeotechnical, @MeasurandVideos) cần được kiểm tra định kỳ 6 tháng/lần để phát hiện video chuyển chế độ private hoặc đổi đường dẫn.
