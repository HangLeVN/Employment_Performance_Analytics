## Employment_Performance_Analytics
# **Chiến lược Quản trị nhân sự và vận hành doanh nghiệp**

## **1. Bối cảnh & Mục tiêu dự án**

**A. Bối cảnh:**

Trong giai đoạn từ năm 2022 đến 2024, doanh thu toàn hệ thống duy trì ở mức ổn định ổn định (~659.77 triệu USD). Tuy nhiên, hoạt động kinh doanh bộc lộ tính chu kỳ rõ rệt (đạt đỉnh vào cuối năm, sụt giảm mạnh vào đầu năm và cuối hè). Đồng thời, doanh nghiệp đang đối mặt với những thách thức ngầm về mặt nhân sự khi tỷ lệ nghỉ việc có xu hướng gia tăng qua các năm (từ 4.95% năm 2022 lên 5.79% năm 2024), gây ảnh hưởng trực tiếp đến hiệu quả vận hành bền vững của tổ chức.

Doanh nghiệp sở hữu quy mô nhân sự lớn với **7,086 nhân viên** phân bổ trên **9 phòng ban** chủ chốt (Store Operations, Logistics/Warehousing, Fresh Produce, Meat/Fish & Bakery, IT, Finance, HR, Marketing, Customer Service), độ tuổi từ 21 - 64 và thâm niên trung bình khoảng 3.5 năm. Mức lương trung bình đạt \$27,253/năm nhưng có sự phân hóa mạnh (75% nhân sự có mức lương dưới \$32,000/năm). Do đó, việc xây dựng một hệ thống phân tích tích hợp dữ liệu giữa Nhân sự (HR Metrics) và Kinh doanh (Business Performance) là vô cùng cấp thiết.

**B. Mục tiêu dự án**
*   **Phân tích toàn diện:** Đánh giá mối quan hệ tương quan giữa lực lượng lao động (giờ đào tạo, tỷ lệ vắng mặt, mức độ hài lòng, thời gian tăng ca) và kết quả kinh doanh trong giai đoạn 2022 - 2024.
*   **Tìm kiếm công thức thành công:** Xác định các động lực cốt lõi giúp tối ưu hóa hiệu suất cho 3 mô hình kinh doanh chính (Đại siêu thị - Superstore, Siêu thị vừa - Regular, Cửa hàng tiện lợi - Express).
*   **Phân loại nguồn lực chiến lược:** Ứng dụng mô hình ma trận để định vị chính xác vị trí của từng nhóm nhân sự (Stars, Core, Risks, Alerts,...) từ đó đưa ra các chiến lược giữ chân và tối ưu năng suất phù hợp.
*   **Đề xuất hành động định hướng 2025:** Cung cấp các khuyến nghị quản trị vận hành mang tính hành động cao ở cả cấp hệ thống lẫn cấp phòng ban.
  
## **2. Techstack (Công cụ sử dụng)**
   Dự án được xây dựng trên nền tảng Python với các thư viện chuyên dụng cho khoa học dữ liệu:
   - Ngôn ngữ: Python
   - Thư viện xử lý dữ liệu: `pandas`, `numpy`, `scipy`
   - Trực quan hóa dữ liệu:
       - `matplotlib` & `seaborn`: Biểu đồ tĩnh và phân tích xu hướng
       - `plotly`:
         
## **3. Insight Chiến lược (Key Insights)**

### A. Công thức thành công theo từng Mô hình Kinh doanh
*   **Superstore (Đại siêu thị - Chiếm 49.59% doanh thu):** Động lực thành công lớn nhất đến từ việc **Tối ưu chuỗi cung ứng và giao hàng đúng hạn (Avg_On_Time_Delivery)** và năng lực điều hành của cấp quản lý (`Avg_manager_performance`).
*   **Regular (Siêu thị vừa - Chiếm 43.59% doanh thu):** Tập trung vào chiến lược **Nâng cao trải nghiệm khách hàng (Avg_Nps_Score)** để tăng tỷ lệ quay lại và giới thiệu.
*   **Express (Cửa hàng tiện lợi - Chiếm 6.46% doanh thu):** Yếu tố quyết định là sự **Linh hoạt tăng cường nhân sự cày cuốc vào giờ cao điểm (Avg_Overtime_Hours)**.

### B. Thực trạng & Nghịch lý Nhân sự
*   **Mức độ hài lòng theo cấp bậc:** Cấp Executive ghi nhận mức độ hài lòng cao nhất, trong khi nhóm **Manager** lại là nhóm có mức độ hài lòng **thấp nhất** toàn hệ thống. Khối Vận hành (Store Operations và Logistics) chia nhau vị trí cao nhất và thấp nhất về độ hài lòng toàn diện.
*   **Nghịch lý tăng ca (Overtime vs Attrition):** Nhân sự làm thêm giờ (OT) nhiều lại có xu hướng ít nghỉ việc hơn nhờ cơ chế chi trả thu nhập sòng phẳng và minh bạch.
*   **Dấu hiệu Quiet Quitting:** Tỷ lệ ngày vắng mặt lặt vặt tăng đột biến chính là chỉ báo hành vi ngắt kết nối (disengagement) rõ ràng nhất trước khi nhân sự chính thức nộp đơn nghỉ việc.
*   **Đào tạo & Hiệu suất:** Dữ liệu chứng minh mối quan hệ tuyến tính đồng biến: Nhân sự được đào tạo càng nhiều giờ, hiệu quả lao động (`Avg_Performance_Rating`) càng cao (áp dụng cho tất cả Job Level & Job Role).

### C. Lý do rời bỏ theo khối phòng ban
*   **Vận hành (Logistics, Store Ops, Fresh Produce):** Rất nhạy cảm với năng lực của cấp lãnh đạo và tính minh bạch của lương OT; việc đào tạo lý thuyết suông không mang lại giá trị giữ chân.
*   **Dịch vụ & Kinh doanh (CS, Marketing):** Cần nền tảng lương cứng vững chắc; đặc biệt nhóm Customer Service có hiện tượng "khảo sát hài lòng nhưng vẫn nghỉ việc" do áp lực trực tiếp từ khách hàng.
*   **Chuyên môn & Kỹ thuật (Finance, IT):** Bộ phận Finance quan tâm đến tần suất tăng lương hơn là lương cứng và dễ nghỉ việc trong im lặng; khối IT quan tâm đặc biệt đến môi trường làm việc, giảm micromanagement và năng lực quản lý trực tiếp.
*   **Nhân sự (HR):** Cực kỳ nhạy cảm với môi trường nội bộ, đòi hỏi môi trường làm việc "toxic-free" và sự gắn kết cao.

## 5. Strategic Recommendations (Khuyến nghị chiến lược năm 2025)

### A. Quản lý Nhân sự - Cấp Hệ thống
1.  **Quản trị tăng ca hợp lý:** Thiết lập hạn mức trần cho giờ OT kết hợp tổ chức các cuộc khảo sát sức khỏe tinh thần định kỳ. Xây dựng kế hoạch tuyển dụng dự phòng để giảm tải cho các giai đoạn cao điểm.
2.  **Đầu tư năng lực Quản lý Cấp trung:** Chuẩn hóa và tài trợ ngân sách đào tạo năng lực quản trị cho các Trưởng phòng, Trưởng nhóm và Store Manager (vì nhóm Manager hiện đang có mức hài lòng thấp nhất).
3.  **Xây dựng Hệ thống Cảnh báo Sớm (Early Warning System):** Gắn cờ vàng cảnh báo tự động trên hệ thống HRIS đối với các nhân sự có số ngày nghỉ lặt vặt tăng đột biến **> 20%** so với trung bình tháng để HR và Line Manager chủ động can thiệp.

### B. Chiến lược hành động theo Phân loại Ma trận Nhân sự
*   **The Stars (662 nhân sự - 11%):** Vạch rõ lộ trình thăng tiến chuyên môn/quản lý, áp dụng cơ chế thưởng nóng và giao các dự án trọng điểm để phát triển kỹ năng lãnh đạo.
*   **The Core (3,805 nhân sự - 61.1%):** Tập trung vào các chương trình nâng cao năng lực (Upskilling) và duy trì động lực làm việc ổn định lâu dài.
*   **The Risks (65 nhân sự - 1.0%):** Tiến hành phỏng vấn giữ chân (Stay Interview) ngay lập tức để tìm hiểu nguyên nhân bất mãn (do lương, môi trường hay thiếu sự công nhận) nhằm đưa ra giải pháp cứu vãn.
*   **Need to Train (1,523 nhân sự - 24.5%):** Đẩy mạnh đào tạo thực chiến và tái thiết kế lại bộ chỉ số KPI phù hợp với năng lực hiện tại của họ.
*   **Need to Pursue (96 nhân sự - 1.5%):** Thúc đẩy các phong trào thi đua nâng cao năng suất, đồng thời khảo sát để cải thiện quy trình làm việc.
*   **The Alert (57 nhân sự - 0.9%):** Thiết lập các mục tiêu ngắn hạn (PIP - Performance Improvement Plan) để giám sát và cải thiện năng suất nghiêm ngặt; thực hiện thay thế nếu không đạt kỳ vọng sau thời gian thử thách.
