# Bike_Sales_Analyst

📘 Tổng quan

Bike Sales Analyst là một dự án phân tích dữ liệu được xây dựng bằng Microsoft Excel, nhằm khám phá hành vi mua xe đạp của khách hàng dựa trên các yếu tố nhân khẩu học và lối sống.
Dự án tập trung vào việc làm sạch dữ liệu, phân tích bằng Pivot Table và xây dựng dashboard tương tác, từ đó rút ra các insight có giá trị giúp doanh nghiệp hiểu rõ khách hàng mục tiêu và tối ưu hóa chiến lược marketing.
Qua dự án này, thể hiện khả năng:
Xử lý và làm sạch dữ liệu
Phân tích dữ liệu thực tế
Trực quan hóa và xây dựng dashboard
Tư duy phân tích và storytelling dữ liệu

🎯 Mục tiêu dự án

Phân tích các yếu tố ảnh hưởng đến quyết định mua xe đạp
Khám phá mối quan hệ giữa độ tuổi, thu nhập, khoảng cách di chuyển và hành vi mua
Xây dựng dashboard trực quan, hỗ trợ ra quyết định nhanh chóng

🧾 Tóm tắt chung về bộ dữ liệu


Bộ dữ liệu bao gồm thông tin khách hàng với các nhóm chính:
Thông tin nhân khẩu học: Gender, Marital Status, Education, Region, Occupation
Yếu tố kinh tế & hành vi: Income, Commute Distance, Cars
Quyết định mua hàng: Purchased Bike (Yes/No)

🧰 Công cụ sử dụng
 
🔹 Python (Data Preprocessing)

Sử dụng Pandas để:
- Làm sạch dữ liệu (xử lý missing values, duplicate)
- Chuẩn hóa kiểu dữ liệu và định dạng (Income, Gender, Marital Status, …)
- Tiền xử lý dữ liệu trước khi đưa vào phân tích

🔹 Microsoft Excel (Analysis & Dashboard)

Data Cleaning:
- Kiểm tra và xử lý dữ liệu không nhất quán
- Chuẩn hóa các trường dữ liệu phục vụ phân tích

Data Analysis:
- Sử dụng Pivot Table để tổng hợp và phân tích dữ liệu
- Thực hiện các phép tính, so sánh giữa các nhóm khách hàng

Data Visualization:
- Pivot Charts (Column, Pie Chart)
- Conditional Formatting để làm nổi bật dữ liệu

Dashboard Design:
- Sử dụng Slicer để tạo bộ lọc tương tác
- Thiết kế layout trực quan, dễ theo dõi
- Trình bày insight rõ ràng, hỗ trợ ra quyết định


📊 Dashboard Features

- Bộ lọc động (Slicer) theo: Gender, Region, Marital Status, Cars

Các biểu đồ chính:
- Thu nhập trung bình 
- Phân bố khoảng cách di chuyển
- Xu hướng mua theo nhóm tuổi
- Tỷ lệ mua theo khu vực (Region)
- Hành vi mua theo số lượng xe sở hữu

Giao diện dashboard:
- Gọn gàng, trực quan
- Tối ưu cho báo cáo và thuyết trình

🔍 Key Insights

1. 🎯 Nhóm khách hàng trọng tâm

Khách hàng trong độ tuổi 31–54 là nhóm có tỷ lệ mua cao nhất và đóng vai trò chính trong doanh số.

2. 🚗 Số lượng xe ảnh hưởng mạnh đến hành vi mua

Khách hàng sở hữu 0–1 xe có xu hướng mua xe đạp cao hơn đáng kể so với nhóm sở hữu nhiều xe.

3. 🚶 Khoảng cách di chuyển là yếu tố quan trọng

Những người có khoảng cách di chuyển ngắn có xu hướng mua xe đạp nhiều hơn, trong khi khoảng cách dài làm giảm nhu cầu.

4. 📍 Thị trường trọng điểm

North America là khu vực chiếm tỷ trọng khách hàng lớn nhất, đóng vai trò là thị trường chính.

5. ⚖️ Thu nhập và giới tính không phải yếu tố quyết định

Sự khác biệt về Income và Gender giữa nhóm mua và không mua là không đáng kể, cho thấy đây không phải là yếu tố phân biệt chính.

🔍 Giải thích 

Phân tích dữ liệu từ dashboard cho thấy nhóm khách hàng trong độ tuổi 31–54 đóng vai trò trung tâm trong hành vi mua xe đạp. Cụ thể, nhóm này ghi nhận 383 khách hàng mua so với 318 khách hàng không mua, chiếm tỷ trọng lớn nhất trong toàn bộ dataset. Trong khi đó, nhóm 0–30 tuổi chỉ có khoảng 39 khách hàng mua, thể hiện nhu cầu rất thấp, còn nhóm trên 54 tuổi có xu hướng ngược lại khi số lượng không mua (130) cao hơn đáng kể so với mua (59). Điều này cho thấy khách hàng trung niên vừa có nhu cầu thực tế vừa có khả năng chi trả, trở thành phân khúc đóng góp chính vào doanh số.

Xét theo số lượng xe sở hữu, dữ liệu cho thấy một xu hướng giảm rõ rệt trong hành vi mua khi số lượng phương tiện tăng lên. Nhóm khách hàng không sở hữu xe (0 cars) có 151 người mua so với 96 người không mua, trong khi nhóm sở hữu 1 xe cũng ghi nhận tỷ lệ mua cao với 152 người mua và 115 người không mua. Tuy nhiên, từ 2 xe trở lên, xu hướng bắt đầu đảo chiều khi số lượng không mua tăng lên đáng kể, điển hình như nhóm 2 xe có 218 người không mua so với 124 người mua. Điều này phản ánh rằng xe đạp thường được xem là phương tiện thay thế hoặc bổ sung cho những người chưa có nhiều phương tiện di chuyển.

Khoảng cách di chuyển hàng ngày cũng là một yếu tố có ảnh hưởng rõ rệt đến hành vi mua. Nhóm khách hàng có khoảng cách 0–1 miles ghi nhận mức mua cao nhất với 200 người, trong khi nhóm 5–10 miles có xu hướng mua nhiều hơn không mua (116 so với 76), tuy nhiên quy mô nhóm này khá nhỏ. Ngược lại, ở khoảng cách trên 10 miles, số lượng khách hàng không mua (78) cao hơn đáng kể so với số lượng mua (33) cho thấy khi khoảng cách di chuyển tăng, tính tiện dụng của xe đạp giảm và nhu cầu theo đó cũng giảm. Nhìn chung, xe đạp phù hợp nhất với các quãng đường ngắn và trung bình.
Về phân bố theo khu vực, dữ liệu cho thấy North America chiếm ưu thế rõ rệt với 508 khách hàng, tương đương khoảng 50.8% tổng số, trong khi Europe có 300 khách hàng (30%) và Pacific chỉ có 192 khách hàng (19.2%). Điều này cho thấy phần lớn hành vi và xu hướng trong dataset chịu ảnh hưởng mạnh từ thị trường North America, đồng thời đây cũng là khu vực tiềm năng nhất để triển khai các chiến lược kinh doanh.

Cuối cùng, xét về thu nhập và giới tính, dữ liệu không cho thấy sự khác biệt đáng kể giữa các nhóm mua và không mua. Thu nhập trung bình của nhóm mua chỉ nhỉnh hơn nhẹ so với nhóm không mua và có sự chồng lấn lớn giữa hai nhóm, trong khi tỷ lệ mua giữa nam và nữ tương đối cân bằng, không có sự lệch đáng kể. Điều này cho thấy Income và Gender không phải là yếu tố phân biệt chính, và hành vi mua xe đạp phụ thuộc nhiều hơn vào các yếu tố liên quan đến lối sống như độ tuổi, số lượng phương tiện và khoảng cách di chuyển.


