<div align="center">

# Thảo Dược Zone — Digital Transformation Project

### Chuyển đổi số Quy trình Bán hàng cho Hộ kinh doanh Trà Thảo dược
**Từ vận hành thủ công đến ra quyết định dựa trên lợi nhuận thực**

![Role](https://img.shields.io/badge/Role-Business%20Analyst-1F3D2B?style=flat-square)
![Status](https://img.shields.io/badge/Status-Completed-6B8F47?style=flat-square)
![Tools](https://img.shields.io/badge/Tools-SQL%20%7C%20Excel%20%7C%20Figma-C97A3D?style=flat-square)
![Case Study](https://img.shields.io/badge/Type-Case%20Study-1F3D2B?style=flat-square)

</div>

---

## Tổng quan

**Thảo Dược Zone** là case study mô phỏng một hộ kinh doanh trà thảo dược tại Việt Nam, bán qua Shopee, TikTok Shop, Zalo/Fanpage và đại lý. Dự án đóng vai trò Business Analyst từ đầu đến cuối: xác định vấn đề nghiệp vụ, thu thập yêu cầu, thiết kế giải pháp, viết BRD/User Story, và **chứng minh insight bằng dữ liệu thật** (SQL trên 1.586 đơn hàng mô phỏng) — thay vì chỉ đề xuất trên giấy.

> **Bối cảnh:** Năm 2026, các sàn TMĐT lớn tại Việt Nam đồng loạt tăng phí, khiến biên lợi nhuận thực tế của hộ kinh doanh nhỏ chỉ còn 5–8%. Thảo Dược Zone không biết chính xác sản phẩm nào đang thực sự có lãi sau khi trừ phí sàn — đây là bài toán dự án này giải quyết.

## Vấn đề nghiệp vụ cốt lõi

| # | Vấn đề | Hệ quả |
|---|---|---|
| 1 | Không biết sản phẩm nào thực sự có lãi | Doanh thu sàn không phản ánh lợi nhuận thực sau phí sàn |
| 2 | Không kiểm soát hạn sử dụng, tồn kho theo lô | Hàng tồn phải bỏ hoặc giảm giá sát hạn |
| 3 | Dữ liệu phân mảnh giữa 4 kênh bán | Ra quyết định dựa trên cảm tính, không có dữ liệu |

## Kết quả nổi bật (từ dữ liệu thật)

Phân tích SQL trên dataset mô phỏng (1.586 đơn hàng, 8 SKU, 3 tháng) cho thấy:

- **Trà cà leo gai giảm cân** — doanh thu cao nhất (24,1 triệu) nhưng **biên lợi nhuận thấp nhất (60,2%)** trong 8 sản phẩm
- **Trà atiso thanh lọc** — doanh thu chỉ bằng 43% sản phẩm trên, nhưng **biên lợi nhuận cao nhất (66,2%)**
- **TikTok Shop** có phí sàn trung bình cao nhất (16%) so với Shopee (13%)

Insight này là căn cứ trực tiếp cho đề xuất tái phân bổ ngân sách marketing theo lợi nhuận thực thay vì chỉ theo doanh thu.

## Cấu trúc repository

| File / Thư mục | Nội dung |
|---|---|
| [`01_Business_Context.docx`](./01_Business_Context.docx) | Bối cảnh doanh nghiệp, bối cảnh thị trường, problem statement |
| [`02_AsIs_Process_Diagram/`](./02_AsIs_Process_Diagram) | Sơ đồ quy trình bán hàng hiện tại, bảng pain points |
| [`03_Stakeholder_Requirement.xlsx`](./03_Stakeholder_Requirement.xlsx) | Stakeholder analysis (Influence/Interest) + Requirement list (MoSCoW) |
| [`04_ToBe_Process_Wireframe/`](./04_ToBe_Process_Wireframe) | Sơ đồ quy trình đề xuất + wireframe 3 màn hình giải pháp |
| [`05_BRD_UserStory.docx`](./05_BRD_UserStory.docx) | Business Requirement Document, Gap Analysis, User Story & Acceptance Criteria |
| [`06_Data_Analysis/`](./06_Data_Analysis) | Database SQLite, SQL queries, dataset CSV, kết quả phân tích |

## Quy trình thực hiện (theo chuẩn BA)

```
Business Context  →  As-Is Process  →  Stakeholder & Requirement
      ↓
To-Be Solution Design  →  Gap Analysis & BRD  →  Data Analysis Demo
      ↓
Recommendation & Roadmap  →  Kết luận & Bài học kinh nghiệm
```

## Công cụ sử dụng

| Hạng mục | Công cụ |
|---|---|
| Tài liệu nghiệp vụ | Google Docs / Word |
| Sơ đồ quy trình | draw.io |
| Wireframe | Figma |
| Phân tích dữ liệu | SQLite, SQL, Excel |
| Quản lý yêu cầu | Excel (Stakeholder & Requirement matrix) |
| Trình bày | PowerPoint |

## Giới hạn của dự án

Dữ liệu trong `06_Data_Analysis/` là **dữ liệu mô phỏng**, được sinh có kiểm soát theo logic nghiệp vụ thực tế (không phải số liệu vận hành thật của một hộ kinh doanh cụ thể), nhằm minh hoạ phương pháp phân tích. Yêu cầu nghiệp vụ được xây dựng dựa trên giả định hợp lý, chưa qua phỏng vấn thực địa.

---

<div align="center">

**Thực hiện bởi Nguyễn Xuân Tú** — Business Analyst

</div>
