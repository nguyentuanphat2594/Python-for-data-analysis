# Phân tích Dữ liệu Bán hàng – Thị trường Đức (Global Superstore)
## Tệp dữ liệu
Nguồn: Global Superstore.xls
Phạm vi phân tích: Chỉ tập trung vào các đơn hàng tại Germany

## Cấu trúc báo cáo
### *1. Tiền xử lý và chuẩn bị dữ liệu*
Lọc dữ liệu theo quốc gia: Germany
Loại bỏ cột dư thừa, xử lý trùng lặp và giá trị thiếu (?, unknown)
Chuẩn hóa định dạng: ngày tháng, số liệu (Sales, Profit, Quantity, ...)
Tạo biến phái sinh:
Profit Margin = Profit / Sales
Delivery Speed = số ngày giữa Order Date và Ship Date
Sales per Customer = trung bình doanh số theo Customer ID

### *2. Thống kê mô tả*
Tổng quan thị trường: số đơn hàng, doanh số, lợi nhuận, số khách hàng
Top thành phố/bang theo doanh số, lợi nhuận, số lượng khách
Phân tích theo:
Danh mục sản phẩm (Category, Sub-Category)
Phân khúc khách hàng (Segment)
Phương thức vận chuyển (Ship Mode)
Độ ưu tiên đơn hàng (Order Priority)

### *3. Trực quan hóa dữ liệu*
Xu hướng doanh số & lợi nhuận theo tháng và quý
Biểu đồ cột: top thành phố, bang, danh mục, phân khúc
Biểu đồ phân tán (scatter): Sales vs Profit
Heatmap: mối quan hệ Category × Segment, lợi nhuận trung bình
Biểu đồ tròn: tỷ lệ khách hàng quay lại, mức độ ưu tiên theo phân khúc & danh mục
Histogram: phân phối thời gian giao hàng
