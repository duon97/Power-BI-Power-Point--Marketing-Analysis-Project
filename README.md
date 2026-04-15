# 📊 Marketing Analytics Project

### Báo cáo Phân tích Hiệu quả Marketing với Power BI
## I. Giới thiệu
# 1. Giới thiệu về Bộ dữ liệu
Dự án này sử dụng bộ dữ liệu Marketing tổng hợp, mô phỏng hoạt động quảng cáo và chiến dịch truyền thông của doanh nghiệp trên nhiều kênh (Google Ads, Facebook Ads, Email Marketing, v.v.).
Bộ dữ liệu bao gồm các thông tin về ngân sách, hiệu suất quảng cáo, tỷ lệ chuyển đổi (Conversion Rate), chi phí trên mỗi lượt click (CPC), doanh thu (Revenue) và lợi nhuận (P&L).

Mục tiêu của dự án là xây dựng Dashboard Power BI giúp đội ngũ Marketing và Ban lãnh đạo chẩn đoán vấn đề hiệu suất, phát hiện nguyên nhân gốc rễ, và đề xuất chiến lược tối ưu hóa ngân sách quảng cáo.

# 2. Giải thích về Bộ dữ liệu (Data Dictionary)
Dữ liệu được tổ chức theo mô hình quan hệ với bảng trung tâm là CampaignPerformance và các bảng danh mục bổ trợ.

Bảng Fact - CampaignPerformance (Hiệu suất Chiến dịch):

CampaignName: Tên chiến dịch quảng cáo.

Channel: Kênh quảng cáo (Google, Facebook, Email, Display, v.v.).

Budget: Ngân sách phân bổ cho chiến dịch.

Spend: Chi phí thực tế đã sử dụng.

Clicks / Impressions: Số lượt click và hiển thị.

CTR / CR: Tỷ lệ click và tỷ lệ chuyển đổi.

Revenue / Profit: Doanh thu và lợi nhuận.

PromotionType: Loại khuyến mãi (Discount, Free Shipping, Promo Code).

Các bảng Dimension (Danh mục):

AudienceSegment: Phân loại nhóm khách hàng mục tiêu.

Seasonality: Ghi nhận yếu tố mùa vụ (Holiday, Sale Season, Launch Period).

AdType: Phân loại hình thức quảng cáo (Video, Banner, Text, Carousel).

# 3. Câu hỏi Kinh doanh (Business Questions)
Hiệu suất tổng thể: Ngân sách quảng cáo được phân bổ như thế nào? Kênh nào mang lại ROI cao nhất?

Phân tích lợi nhuận: Có mối tương quan nào giữa chi tiêu quảng cáo (Ad Spend) và lợi nhuận (P&L)?

Tối ưu hóa ngân sách: Các chiến dịch có ngân sách cao có thực sự mang lại hiệu quả tương xứng không?

Hiệu quả khuyến mãi: Loại khuyến mãi nào (Discount, Free Shipping, Promo Code) tạo ra tỷ lệ chuyển đổi cao nhất?

Phân khúc khách hàng: Nhóm khách hàng nào có mức độ tương tác (Engagement) và chuyển đổi tốt nhất?

## II. Phương pháp Tư duy Thiết kế (Design Thinking Method)
* Empathize (Thấu cảm): Đặt mình vào góc nhìn của Giám đốc Marketing (CMO) – người cần hiểu rõ nguyên nhân khiến ROI giảm và xác định chiến dịch nào đang tiêu tốn ngân sách mà không mang lại lợi nhuận.

* Define (Xác định vấn đề): Xác định các chỉ số cốt lõi (KPIs): Total Spend, ROI, CTR, CR, Profit Margin, Ad Engagement, Budget Utilization.

* Ideate (Lên ý tưởng):
<img width="1242" height="848" alt="marketing" src="https://github.com/user-attachments/assets/ad5120fd-10c0-4a1c-a4a6-7c31f8edaa53" />



* Prototype (Xây dựng mô hình):

    Data Preparation: Làm sạch dữ liệu, chuẩn hóa định dạng ngày tháng, xử lý giá trị null.


    DAX: Tạo các Measures tính ROI, CTR trung bình, và tỷ lệ lợi nhuận.

* Test (Kiểm thử): Đảm bảo các bộ lọc hoạt động mượt mà, biểu đồ tương tác tốt, và giao diện trực quan dễ hiểu.


## III. Trực quan hóa Dữ liệu trên Powerpoint (Visualization), Xây dựng dashboard theo dõi hiệu suất
Trang 1: Marketing Overview (Tổng quan Hiệu suất)  
Hiển thị các KPI chính: Total Spend, ROI, CTR, CR, Profit Margin.  
<img width="1315" height="739" alt="image" src="https://github.com/user-attachments/assets/ebc0e8fd-c389-447a-bd2c-4433643ce729" />

Trang 2: Campaign Diagnosis (Chi tiết về P&L, Impression, Click, CTR... trong từng tháng)  

<img width="1319" height="734" alt="image" src="https://github.com/user-attachments/assets/b90eee17-b420-4b58-8b49-7f4336f5871b" />

## IV. Thông tin Chi tiết (Insights)
**  Về Hiệu suất Chiến dịch:

* Chi tiêu tối ưu thúc đẩy lợi nhuận.
<img width="1238" height="696" alt="image" src="https://github.com/user-attachments/assets/14805136-f36a-48fe-94f6-46e21c1f6cfd" />
Tháng 10 cho thấy việc kiểm soát ngân sách hợp lý đã giúp P&L dương. Điều này nhấn mạnh rằng chi tiêu chiến lược quan trọng hơn việc tăng chi tiêu đơn thuần.

* Khuyến mãi giảm giá bị lạm dụng

Các chương trình khuyến mãi và mã giảm giá chiếm tới 88% ngân sách, cho thấy doanh nghiệp quá phụ thuộc vào ưu đãi trực tiếp, trong khi các chiến dịch mùa vụ chưa được khai thác đúng mức.
<img width="1225" height="434" alt="image" src="https://github.com/user-attachments/assets/ca687d82-1449-4a2d-bec4-41681cbea3be" />

* Chi nhiều ≠ Lợi nhuận cao
<img width="1211" height="412" alt="image" src="https://github.com/user-attachments/assets/cb222655-1ace-4de7-b484-a9759b080c57" />
<img width="1149" height="461" alt="image" src="https://github.com/user-attachments/assets/93c2f79f-39ec-4495-9d81-ad741ee1088a" />

* Phân khúc & nội dung quảng cáo là yếu tố quyết định
CTR và CR không tỷ lệ thuận, chứng minh rằng cần cải thiện phân khúc khách hàng và tối ưu hóa nội dung quảng cáo để nâng cao hiệu quả chuyển đổi.
<img width="463" height="288" alt="image" src="https://github.com/user-attachments/assets/a1248cc0-6f37-4866-94c4-d11d1457a126" />



## V. Đề xuất & Khuyến nghị (Recommendations)
Tối ưu hóa ngân sách: Giảm ngân sách cho các chiến dịch có ROI thấp, chuyển hướng sang kênh có hiệu quả cao hơn.

Cải thiện nội dung quảng cáo: Tập trung vào tối ưu hóa thông điệp và định dạng video để tăng CTR.

Chiến lược khuyến mãi thông minh: Kết hợp “Promo Code” với “Limited-Time Offer” để vừa tăng chuyển đổi vừa duy trì lợi nhuận.

Phân tích theo mùa vụ: Tăng cường chiến dịch vào các giai đoạn cao điểm (Holiday, Sale Season) để tận dụng hành vi mua sắm.

Xây dựng hệ thống giám sát hiệu suất: Thiết lập Dashboard theo thời gian thực để phát hiện sớm các chiến dịch kém hiệu quả và điều chỉnh kịp thời.


