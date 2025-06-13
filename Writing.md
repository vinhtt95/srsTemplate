# Căn bản

1.  Rõ ràng
2.  Ngắn gọn
3.  Trung thực
4.  Thân thiện
5.  Có ích

# Một yêu cầu xuất sắc

## 1\. Hoàn chỉnh

Một yêu cầu phải chứa tất cả thông tin cần thiết để người đọc hiểu nó.

\* Đối với yêu cầu chức năng: Cần cung cấp đủ thông tin cần thiết để dev có thể **triển khai đúng**.

\* Nếu phần thông tin bị thiếu, cần đánh dấu để theo dõi và lên kế hoạch hoàn chỉnh trước khi bắt đầu triển khai thực hiện.

## 2\. Đúng đắn

Yêu cầu phải mô tả chính xác một khả năng đáp ứng nhu cầu của một bên liên quan (stakeholder) và mô tả rõ ràng chức năng cần xây dựng.

\* Cần kiểm tra nguồn gốc của yêu cầu xuất phát từ đâu. Đảm bảo không có sự xung đột với yêu cầu cấp cao hơn.

## 3\. Khả thi

Yêu cầu phải có thể triển khai trong phạm vi khả năng và giới hạn đã biết của hệ thống và môi trường vận hành, cũng như trong các ràng buộc của dự án.

## 4\. Cần thiết

Yêu cầu nên mô tả một khả năng mang lại giá trị kinh doanh dự kiến cho các bên liên quan, tạo sự khác biệt cho sản phẩm trên thị trường hoặc cần thiết để tuân thủ tiêu chuẩn, chính sách hoặc quy định bên ngoài.

## 5\. Ưu tiên

Dựa trên mức độ quan trọng đối với các giá trị mong muốn mà xác định mức độ ưu tiên của yêu cầu.

## 6\. Không mơ hồ

Đảm bảo tất cả người đọc đều hiểu chung một ý đang được yêu cầu mô tả.

## 7\. Có thể kiểm chứng

Yêu cầu phải cụ thể, có thể do lường, xác minh được. Nghĩa là tester có thể kiểm chứng được yêu cầu thông qua các bài kiểm tra.

# Một tập hợp yêu cầu xuất sắc

## 1\. Hoàn chỉnh

Không yêu cầu hoặc thông tin cần thiết nào bị thiếu. Hạn chế tối đa các yêu cầu giả định hoặc ngụ ý.

## 2\. Nhất quán

Không yêu cầu nào mâu thuẫn với các yêu cầu khác cùng loại hoặc yêu cầu cấp cao hơn.

## 3\. Có thể sửa đổi

Mỗi yêu cầu được gắn nhãn duy nhất và được diễn đạt riêng biệt để có thể tham chiếu không mơ hồ.

## 4\. Có thể truy vết

Có thể được liên kết ngược về nguồn gốc và tiến tới các yêu cầu dẫn xuất, thành phần thiết kế, mã triển khai, và bài kiểm tra xác minh.

# Cách viết

> Giao tiếp/ truyền đạt hiệu quả là mục tiêu bao quát, miễn là yêu cầu được diễn đạt rõ ràng.

Có thể viết yêu cầu từ góc nhìn của hệ thống hoặc của người dùng

*   Hệ thống: \[Điều kiện tiên quyết tùy chọn\] \[sự kiện kích hoạt tùy chọn\] hệ thống phải \[phản hồi hệ thống dự kiến\]
    *   Ví dụ: _Nếu hóa chất yêu cầu được tìm thấy trong kho hóa chất, hệ thống phải hiển thị danh sách tất cả các thùng chứa hóa chất hiện có trong kho._
*   Người dùng: _\[Loại người dùng hoặc tên tác nhân\] phải có thể \[làm gì đó\] \[với đối tượng nào đó\] \[điều kiện định tính, thời gian phản hồi, hoặc tuyên bố về chất lượng\]_
    *   _Ví dụ: Người mua hàng phải có thể đặt lại bất kỳ hóa chất nào anh ta đã đặt trước đây bằng cách truy xuất và chỉnh sửa chi tiết đơn hàng._

_Sử dụng giọng văn chủ động (chỉ rõ đối tượng thực hiền hành động)_

*   Đúng: **H**_**ệ thống** phải cập nhật hợp đồng của khách hàng với số seri sản phẩm mới._
*   _Sai: Số seri sẽ được cập nhật trên dòng hợp đồng. (Ai / cái gì cập nhật số seri?)_

Tách nhỏ thành các yêu cầu riêng lẻ

*   Hạn chế sử dụng các từ: và, hoặc, thêm vào đó, bên cạnh đó, cũng ... nhằm gợi ý các sự kết hợp yêu cầu.
    *   Ví dụ: _Hệ thống phải cho phép tìm kiếm theo số đơn hàng, số hóa đơn, và/hoặc số đơn đặt hàng của khách hàng._
*   Hạn chế các từ: trừ khi, ngoại trừ, nhưng ... 
    *   Ví dụ: _Thẻ tín dụng của Người mua trong hồ sơ phải được sử dụng để thanh toán, **trừ khi** thẻ tín dụng đã hết hạn._ (Nếu vào trường hợp trừ khi thì hệ thống sẽ phản ứng thế nào?)
    *   _Thay vào đó hãy tách làm 2 yêu cầu:_
        *   _Nếu thẻ tín dụng của Người mua trong hồ sơ còn hoạt động, hệ thống phải tính thanh toán vào thẻ đó._
        *   _Nếu thẻ tín dụng của Người mua trong hồ sơ đã hết hạn, hệ thống phải cho phép Người mua cập nhật thông tin thẻ hiện tại hoặc nhập thẻ tín dụng mới để thanh toán._

Tránh các từ ngữ mơ hồ: Chấp nhận được, vừa đủ, nhiều nhất có thể, tối thiểu, ít nhất,...

# Mẫu

_Trình kiểm tra thiết bị (device tester) phải cho phép người dùng dễ dàng kết nối các thành phần bổ sung, bao gồm máy tạo xung (pulse generator), vôn kế (voltmeter), máy đo điện dung (capacitance meter), và thẻ đầu dò tùy chỉnh (custom probe cards)._

Yêu cầu này dành cho một sản phẩm chứa phần mềm nhúng dùng để kiểm tra nhiều loại thiết bị đo lường. Từ "dễ dàng" (easily) ngụ ý một yêu cầu về tính dễ dùng (usability requirement), nhưng nó không thể đo lường hoặc kiểm chứng. "Bao gồm" (including) không làm rõ liệu đây là danh sách đầy đủ các thiết bị bên ngoài phải được kết nối với trình kiểm tra. Có thể có nhiều thiết bị khác mà chúng ta không biết. Hãy xem xét các yêu cầu thay thế sau, chứa một số ràng buộc thiết kế cố ý:

1.  _Trình kiểm tra thiết bị phải tích hợp một cổng USB để cho phép người dùng kết nối bất kỳ thiết bị đo lường nào có kết nối USB._
2.  _Cổng USB phải được cài đặt trên bảng điều khiển phía trước để cho phép một người vận hành được đào tạo kết nối thiết bị đo lường trong 10 giây hoặc ít hơn._

BA không nên viết lại yêu cầu theo cách áp đặt ràng buộc thiết kế theo sáng kiến của mình. Thay vào đó, hãy phát hiện yêu cầu có lỗi và thảo luận với các bên liên quan phù hợp để làm rõ chúng.