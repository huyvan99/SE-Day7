# SE-Day7
Phần Mềm Quản Lý Khách Sạn

# 1. Goals
- Xây dựng phần mềm hoạt động trên máy tính cho 3 đối tượng sử dụng sau: Nhân viên lễ tân, Nhân viên bán hàng, Quản lí.
- Mô hình khách sạn: tên, địa chỉ, đánh giá chấm sao (text và ảnh)
    + Mỗi phòng trong khách sạn được mô tả bằng các thông tin: tên phòng (duy nhất, để phân biệt các phòng), loại phòng, giá niêm yết, các loại dịch vụ đi kèm, mô tả phòng.
    + Mỗi phòng có thể được đặt/ở bởi nhiều khách hàng khác nhau tại những thời điểm khác nhau.
-	Khách hàng:
    + Khi đến ở hoặc đặt phòng, sẽ được lưu các thông tin bao gồm số CMND (số passport nếu là người nước ngoài), loại giấy tùy thân (CMND, passport), họ tên đầy đủ, địa chỉ, số điện thoại, ghi chú về phục vụ đặc biệt như cho người khuyết tật, ăn chay...
    + Mỗi khách hàng có thể đặt/ở nhiều phòng khác nhau tại những thời điểm khác nhau.
    + Tại một thời điểm, chỉ có một khách ở trong một phòng, và xác định một giá phòng cụ thể.
    + Khách hàng chỉ có thể đặt phòng nếu phòng đó còn trống trong suốt thời gian khách hàng muốn đặt.
    + Khách hàng có thể thanh toán nhiều lần cho đến ngày trả phòng.
-	Mỗi lần thanh toán, lễ tân sẽ in hóa đơn cho lần thanh toán đó bao gồm các thông tin: họ tên và địa chỉ khách hàng, số phòng, ngày đến, ngày đi, giá phòng, các dịch vụ đi kèm (mỗi dịch vụ bao gồm tên dịch vụ, đơn vị tính, đơn giá, tổng tiền), số tiền thanh toán.
-	Khách hàng có thể hủy đặt phòng (miên phí) nếu hủy trước ngày đến. Nếu khách hàng hủy sau ngày đặt thì khách hàng bị lưu vào danh sách đen và có thể bị từ chối đặt phòng trong các lần tiếp theo

# 2. Business Objectives
- Mục tiêu doanh thu: Bán với giá ưu đãi để tạo mối quan hệ, qua đó có thể tiếp tục hợp tác và bán cho nhiều khách sạn khác.
- Mục tiêu hoạt động: Tạo chuối liên kết. Ví dụ Cung - Cầu: kết nối khách sạn với khách hàng thông qua các phần mềm, chạy quảng cáo của công ty, app trên điện thoại... Khi có một số lượng khách sạn ổn định sử dụng có thể đưa ra một vài cải tiến cho phần mềm. Ví dụ: ứng dụng thêm công nghệ, liên kết để khách hàng dễ dàng chọn lựa dịch vụ của khách sạn hơn.
- Năng suất và hiệu quả hoạt động: Nhân viên là mạch máu của doanh nghiệp. Nhân viên làm việc hiệu quả sẽ thúc đẩy doanh thu và cải thiện sự hài lòng của khách hàng. Đo lường sự hài lòng của nhân viên và thiết lập mục tiêu cho mỗi nhóm chắc chắn sẽ góp phần quan trọng đảm bảo hiệu quả và năng suất.
- Sự hài lòng của khách hàng: Khách hàng luôn là ưu tiên hàng đầu trong bất kỳ doanh nghiệp nào. Một doanh nghiệp thường xuyên khảo sát khách hàng của họ sẽ có thể chắc chắn hơn rằng họ đang tạo hình ảnh tốt trong mắt khách hàng. Muốn cải tiến và bán được sản phẩm chắc chắn phải lắng nghe trải nghiệm của người dùng.
- Tăng trưởng: Các công ty đo lường sự tăng trưởng trong dài hạn và ngắn hạn. Tăng trưởng xuất hiện dưới dạng số lượng khách sạn đặt hàng, doanh thu, trải nghiệm khách hàng...
