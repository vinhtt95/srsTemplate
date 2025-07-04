# **1\. Introduction**

Phần giới thiệu trình bày một cái nhìn tổng quan để giúp người đọc hiểu cách tổ chức SRS và cách sử dụng nó.

## **1.1 Purpose**

Xác định sản phẩm hoặc ứng dụng mà yêu cầu của nó được đặc tả trong tài liệu này, bao gồm số phiên bản hoặc bản phát hành. Nếu SRS này chỉ liên quan đến một phần của một hệ thống phức tạp, hãy xác định phần hoặc hệ thống con đó. Mô tả các loại người đọc khác nhau mà tài liệu này hướng đến, như nhà phát triển, quản lý dự án, nhân viên tiếp thị, người dùng, người kiểm thử, và người viết tài liệu.  

## **1.2 Document conventions**

Mô tả bất kỳ tiêu chuẩn hoặc quy ước typographical nào được sử dụng, bao gồm ý nghĩa của các kiểu văn bản cụ thể, đánh dấu, hoặc ký hiệu. Nếu bạn đang gắn nhãn yêu cầu thủ công, bạn có thể chỉ định định dạng ở đây cho bất kỳ ai cần thêm sau này.  

## **1.3 Project scope**

Cung cấp một mô tả ngắn về phần mềm đang được đặc tả và mục đích của nó. Liên kết phần mềm với các mục tiêu của người dùng hoặc doanh nghiệp và với các mục tiêu và chiến lược kinh doanh. Nếu có một tài liệu vision and scope document (tài liệu tầm nhìn và phạm vi) riêng, hãy tham chiếu đến nó thay vì sao chép nội dung của nó ở đây. Một SRS đặc tả một bản phát hành tăng dần của một sản phẩm đang phát triển nên chứa tuyên bố phạm vi riêng của nó như một tập hợp con của tầm nhìn sản phẩm chiến lược dài hạn. Bạn có thể cung cấp một tóm tắt cấp cao về các tính năng chính mà bản phát hành chứa hoặc các chức năng quan trọng mà nó thực hiện.  

## **1.4 References**

Liệt kê bất kỳ tài liệu hoặc nguồn tài nguyên nào mà SRS này tham chiếu. Bao gồm các siêu liên kết đến chúng nếu chúng ở vị trí cố định. Những thứ này có thể bao gồm hướng dẫn kiểu giao diện người dùng, hợp đồng, tiêu chuẩn, system requirements specification (đặc tả yêu cầu hệ thống), đặc tả giao diện, hoặc SRS cho một sản phẩm liên quan. Cung cấp đủ thông tin để người đọc có thể truy cập mỗi tài liệu tham khảo, bao gồm tiêu đề, tác giả, số phiên bản, ngày, nguồn, vị trí lưu trữ, hoặc URL.

# **2\. Overall description**

Phần này trình bày một cái nhìn tổng quan cấp cao về sản phẩm và môi trường mà nó sẽ được sử dụng, các người dùng dự kiến, và các ràng buộc, giả định, và phụ thuộc đã biết.

## **2.1 Product perspective**

Mô tả bối cảnh và nguồn gốc của sản phẩm. Nó có phải là thành viên tiếp theo của một dòng sản phẩm đang phát triển, phiên bản tiếp theo của một hệ thống trưởng thành, thay thế cho một ứng dụng hiện có, hay một sản phẩm hoàn toàn mới? Nếu SRS này định nghĩa một thành phần của một hệ thống lớn hơn, hãy nêu cách phần mềm này liên quan đến toàn bộ hệ thống và xác định các giao diện chính giữa hai bên. Cân nhắc bao gồm các mô hình trực quan như sơ đồ ngữ cảnh hoặc bản đồ hệ sinh thái để hiển thị mối quan hệ của sản phẩm với các hệ thống khác.

## **2.2 User classes and characteristics**

Xác định các lớp người dùng khác nhau mà bạn dự đoán sẽ sử dụng sản phẩm này, và mô tả các đặc điểm liên quan của họ. Một số yêu cầu có thể chỉ liên quan đến một số lớp người dùng nhất định. Xác định các lớp người dùng được ưu tiên. Các lớp người dùng đại diện cho một tập hợp con của các bên liên quan được mô tả trong vision and scope document (tài liệu tầm nhìn và phạm vi). Các mô tả lớp người dùng là một nguồn tài nguyên có thể tái sử dụng. Nếu có một danh mục lớp người dùng chính, bạn có thể kết hợp các mô tả lớp người dùng bằng cách chỉ vào chúng trong danh mục thay vì sao chép thông tin ở đây.

<table><tbody><tr><td>User Class 1</td><td>Mô tả ngắn</td></tr><tr><td>User Class 2</td><td>Mô tả ngắn</td></tr><tr><td>User Class 3</td><td>Mô tả ngắn</td></tr><tr><td>User Class 4</td><td>Mô tả ngắn</td></tr></tbody></table>

## **2.3 Operating environment**

Mô tả môi trường mà phần mềm sẽ hoạt động, bao gồm nền tảng phần cứng; hệ điều hành và phiên bản; vị trí địa lý của người dùng, máy chủ, và cơ sở dữ liệu; và các tổ chức lưu trữ các cơ sở dữ liệu, máy chủ, và trang web liên quan. Liệt kê bất kỳ thành phần hoặc ứng dụng phần mềm nào khác mà hệ thống phải cùng tồn tại hòa bình. Nếu cần thực hiện công việc cơ sở hạ tầng kỹ thuật rộng rãi cùng với việc phát triển hệ thống mới, hãy cân nhắc tạo một đặc tả yêu cầu cơ sở hạ tầng riêng để chi tiết hóa công việc đó.

## **2.4 Design and implementation constraints**

Có những lúc một ngôn ngữ lập trình nhất định phải được sử dụng, một thư viện mã cụ thể đã được đầu tư thời gian để phát triển cần được sử dụng, v.v. Mô tả bất kỳ yếu tố nào sẽ hạn chế các lựa chọn có sẵn cho các nhà phát triển và lý do cho mỗi ràng buộc. Các yêu cầu kết hợp hoặc được viết dưới dạng ý tưởng giải pháp thay vì nhu cầu đang áp đặt các ràng buộc thiết kế, thường không cần thiết, vì vậy hãy cẩn thận với những điều đó.   

## **2.5 Assumptions and dependencies**

Một giả định là một tuyên bố được tin là đúng khi không có bằng chứng hoặc kiến thức xác định. Các vấn đề có thể phát sinh nếu các giả định không chính xác, lỗi thời, không được chia sẻ, hoặc thay đổi, vì vậy một số giả định sẽ chuyển thành rủi ro dự án. Một người đọc SRS có thể giả định rằng sản phẩm sẽ tuân theo một quy ước giao diện người dùng cụ thể, trong khi một người khác có thể giả định điều gì đó khác. Một nhà phát triển có thể giả định rằng một tập hợp chức năng sẽ được viết tùy chỉnh cho ứng dụng này, trong khi nhà phân tích kinh doanh có thể giả định rằng chúng sẽ được tái sử dụng từ một dự án trước, và quản lý dự án có thể mong đợi mua một thư viện chức năng thương mại. Các giả định cần đưa vào đây là những giả định liên quan đến chức năng hệ thống; các giả định liên quan đến kinh doanh xuất hiện trong vision and scope document (tài liệu tầm nhìn và phạm vi).  
Xác định bất kỳ phụ thuộc nào mà dự án hoặc hệ thống đang được xây dựng có trên các yếu tố hoặc thành phần bên ngoài ngoài tầm kiểm soát của nó. Ví dụ, nếu Microsoft .NET Framework 4.5 hoặc phiên bản mới hơn phải được cài đặt trước khi sản phẩm của bạn có thể chạy, đó là một phụ thuộc.

# **3\. System features**

Mẫu trong Hình 10-2 hiển thị các functional requirement (yêu cầu chức năng) được tổ chức theo tính năng hệ thống, chỉ là một cách tổ chức có thể có. Các lựa chọn tổ chức khác bao gồm sắp xếp các functional requirement (yêu cầu chức năng) theo lĩnh vực chức năng, luồng quy trình, use case (trường hợp sử dụng), chế độ vận hành, lớp người dùng, kích thích, và phản hồi. Các kết hợp phân cấp của các yếu tố này cũng có thể, chẳng hạn như các use case (trường hợp sử dụng) trong các lớp người dùng. Không có lựa chọn đúng duy nhất; hãy chọn một phương pháp tổ chức giúp người đọc dễ dàng hiểu các khả năng dự định của sản phẩm. Chúng tôi sẽ mô tả sơ đồ tính năng như một ví dụ.

## **3.1 System feature X**

Nêu tên của tính năng trong vài từ, chẳng hạn như "3.1 Kiểm tra chính tả." Lặp lại phần 3.x với các tiểu mục 3.x.1 và 3.x.2 cho mỗi tính năng hệ thống.

### **3.1.1 Description**

Cung cấp một mô tả ngắn về tính năng và chỉ ra liệu nó có mức độ ưu tiên cao, trung bình hay thấp. Các ưu tiên thường thay đổi trong suốt dự án. Nếu bạn đang sử dụng một requirements management tool (công cụ quản lý yêu cầu), hãy định nghĩa một thuộc tính yêu cầu cho ưu tiên.  

### **3.1.2 Functional requirements**

Liệt kê các functional requirement (yêu cầu chức năng) cụ thể liên quan đến tính năng này. Đây là những khả năng phần mềm phải được triển khai để người dùng thực hiện các dịch vụ của tính năng hoặc thực hiện một use case (trường hợp sử dụng). Mô tả cách sản phẩm nên phản ứng với các điều kiện lỗi dự kiến và các đầu vào và hành động không hợp lệ. Gắn nhãn duy nhất cho mỗi functional requirement (yêu cầu chức năng). Nếu bạn đang sử dụng một requirements management tool (công cụ quản lý yêu cầu), bạn có thể tạo nhiều thuộc tính cho mỗi functional requirement (yêu cầu chức năng), như lý do, nguồn gốc, và trạng thái.  
 

<table><tbody><tr><td colspan="2"><strong>Name.Of.Func1</strong></td></tr><tr><td>.Create:</td><td>Mô tả</td></tr><tr><td>.Update:</td><td>Mô tả</td></tr><tr><td colspan="2"><strong>Name.Of.Func2</strong></td></tr><tr><td>.Create:</td><td>Mô tả</td></tr><tr><td>.Update:</td><td>Mô tả</td></tr><tr><td>.View:</td><td>Mô tả</td></tr><tr><td>.Delete:</td><td>Mô tả</td></tr></tbody></table>

# **4\. Data requirements**

Hệ thống thông tin cung cấp giá trị bằng cách thao tác dữ liệu. Sử dụng phần này của mẫu để mô tả các khía cạnh khác nhau của dữ liệu mà hệ thống sẽ tiêu thụ dưới dạng đầu vào, xử lý theo một cách nào đó, hoặc tạo ra dưới dạng đầu ra.

## **4.1 Logical data model**

Mô hình dữ liệu là một biểu diễn trực quan của các đối tượng và bộ sưu tập dữ liệu mà hệ thống sẽ xử lý và các mối quan hệ giữa chúng. Có nhiều ký hiệu cho mô hình hóa dữ liệu, bao gồm sơ đồ mối quan hệ thực thể (entity-relationship diagrams) và sơ đồ lớp UML. Bạn có thể bao gồm một mô hình dữ liệu cho các hoạt động kinh doanh được giải quyết bởi hệ thống, hoặc một biểu diễn logic cho dữ liệu mà hệ thống sẽ thao tác. Đây không phải là mô hình dữ liệu triển khai sẽ được hiện thực hóa dưới dạng thiết kế cơ sở dữ liệu.

## **4.2 Data dictionary**

Từ điển dữ liệu định nghĩa thành phần của các cấu trúc dữ liệu và ý nghĩa, kiểu dữ liệu, độ dài, định dạng, và các giá trị được phép cho các phần tử dữ liệu tạo nên các cấu trúc đó. Các công cụ mô hình hóa dữ liệu thương mại thường bao gồm một thành phần từ điển dữ liệu. Trong nhiều trường hợp, bạn nên lưu trữ từ điển dữ liệu như một hiện vật riêng biệt, thay vì nhúng nó vào giữa SRS. Điều này cũng làm tăng tiềm năng tái sử dụng trong các dự án khác.

<table><tbody><tr><td><p style="text-align:center;"><strong>Data Element</strong></p></td><td><p style="text-align:center;"><strong>Description</strong></p></td><td><p style="text-align:center;"><strong>Composition or Data Type</strong></p></td><td><p style="text-align:center;"><strong>Length</strong></p></td><td><p style="text-align:center;"><strong>Values</strong></p></td></tr><tr><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td></tr></tbody></table>

## **4.3 Reports**

Nếu ứng dụng của bạn sẽ tạo ra bất kỳ báo cáo nào, hãy xác định chúng ở đây và mô tả các đặc điểm của chúng. Nếu một báo cáo phải tuân theo một bố cục được xác định trước cụ thể, bạn có thể chỉ định điều đó ở đây như một ràng buộc, có thể với một ví dụ. Nếu không, hãy tập trung vào các mô tả logic của nội dung báo cáo, trình tự sắp xếp, các mức tổng hợp, v.v., hoãn bố cục báo cáo chi tiết sang giai đoạn thiết kế.

<table><tbody><tr><td><p style="text-align:right;">Report ID:</p></td><td>&nbsp;</td></tr><tr><td><p style="text-align:right;">Report Title:</p></td><td>&nbsp;</td></tr><tr><td><p style="text-align:right;">Report Purpose:</p></td><td>&nbsp;</td></tr><tr><td><p style="text-align:right;">Priority:</p></td><td>&nbsp;</td></tr><tr><td><p style="text-align:right;">Report Users:</p></td><td>&nbsp;</td></tr><tr><td><p style="text-align:right;">Data Sources:</p></td><td>&nbsp;</td></tr><tr><td><p style="text-align:right;">Frequency and Disposition;</p></td><td>&nbsp;</td></tr><tr><td><p style="text-align:right;">Latency:</p></td><td>&nbsp;</td></tr><tr><td><p style="text-align:right;">Visual Layout:</p></td><td>&nbsp;</td></tr><tr><td><p style="text-align:right;">Header and Footer:</p></td><td>&nbsp;</td></tr><tr><td><p style="text-align:right;">Report Body:</p></td><td>&nbsp;</td></tr><tr><td><p style="text-align:right;">End-of-Report Indicator:</p></td><td>&nbsp;</td></tr><tr><td><p style="text-align:right;">Interactivity:</p></td><td>&nbsp;</td></tr><tr><td><p style="text-align:right;">Security Access Restrictions:</p></td><td>&nbsp;</td></tr></tbody></table>

## **4.4 Data acquisition, integrity, retention, and disposal**

Nếu phù hợp, mô tả cách dữ liệu được thu thập và duy trì. Ví dụ, khi bắt đầu một luồng dữ liệu tồn kho, bạn có thể cần thực hiện một lần đổ toàn bộ dữ liệu tồn kho vào hệ thống nhận và sau đó có các luồng tiếp theo chỉ gồm các thay đổi. Nêu bất kỳ yêu cầu nào liên quan đến việc bảo vệ tính toàn vẹn của dữ liệu hệ thống. Xác định bất kỳ kỹ thuật cụ thể nào cần thiết, như sao lưu, điểm kiểm tra, sao chép, hoặc xác minh độ chính xác dữ liệu. Nêu các chính sách mà hệ thống phải thực thi để lưu giữ hoặc loại bỏ dữ liệu, bao gồm dữ liệu tạm thời, siêu dữ liệu, dữ liệu còn lại (như các bản ghi đã bị xóa), dữ liệu được lưu vào bộ đệm, bản sao cục bộ, kho lưu trữ, và các bản sao lưu tạm thời.

# **5\. External interface requirements**

Phần này cung cấp thông tin để đảm bảo rằng hệ thống sẽ giao tiếp đúng cách với người dùng và với các phần tử phần cứng hoặc phần mềm bên ngoài. Việc đạt được thỏa thuận về các giao diện hệ thống bên ngoài và nội bộ đã được xác định là một thực hành tốt nhất trong ngành phần mềm (Brown 1996). Một hệ thống phức tạp với nhiều thành phần phụ nên tạo một đặc tả giao diện riêng hoặc đặc tả kiến trúc hệ thống. Tài liệu giao diện có thể kết hợp tài liệu từ các tài liệu khác bằng cách tham chiếu. Ví dụ, nó có thể trỏ đến một hướng dẫn thiết bị phần cứng liệt kê các mã lỗi mà thiết bị có thể gửi đến phần mềm.

## **5.1 User interfaces**

Mô tả các đặc điểm logic của mỗi giao diện người dùng mà hệ thống cần. Một số đặc điểm cụ thể của giao diện người dùng có thể xuất hiện trong phần 6.1 Tính khả dụng. Một số mục có thể được đề cập ở đây bao gồm:

*   Tham chiếu đến các tiêu chuẩn giao diện người dùng hoặc hướng dẫn kiểu dòng sản phẩm cần tuân theo.
*   Tiêu chuẩn cho phông chữ, biểu tượng, nhãn nút, hình ảnh, bảng màu, trình tự tab trường, các điều khiển thường dùng, đồ họa thương hiệu, thông báo bản quyền và quyền riêng tư, v.v.
*   Ràng buộc về kích thước màn hình, bố cục, hoặc độ phân giải.
*   Các nút tiêu chuẩn, chức năng, hoặc liên kết điều hướng sẽ xuất hiện trên mọi màn hình, như nút trợ giúp.
*   Phím tắt.
*   Quy ước hiển thị và diễn đạt thông báo.
*   Hướng dẫn xác thực dữ liệu (như hạn chế giá trị đầu vào và khi nào xác thực nội dung trường).
*   Tiêu chuẩn bố cục để hỗ trợ bản địa hóa phần mềm.
*   Các điều chỉnh cho người dùng bị khiếm thị, mù màu, hoặc có các hạn chế khác.

## **5.2 Software interfaces**

Mô tả các kết nối giữa sản phẩm này và các thành phần phần mềm khác (được xác định bằng tên và phiên bản), bao gồm các ứng dụng khác, cơ sở dữ liệu, hệ điều hành, công cụ, thư viện, trang web, và các thành phần thương mại tích hợp. Nêu mục đích, định dạng, và nội dung của các thông điệp, dữ liệu, và giá trị điều khiển được trao đổi giữa các thành phần phần mềm. Chỉ định các ánh xạ của dữ liệu đầu vào và đầu ra giữa các hệ thống và bất kỳ bản dịch nào cần được thực hiện để dữ liệu di chuyển từ hệ thống này sang hệ thống khác. Mô tả các dịch vụ cần bởi hoặc từ các thành phần phần mềm bên ngoài và bản chất của các giao tiếp giữa các thành phần. Xác định dữ liệu sẽ được trao đổi giữa hoặc chia sẻ trên các thành phần phần mềm. Chỉ định các nonfunctional requirement (yêu cầu phi chức năng) ảnh hưởng đến giao diện, như mức dịch vụ cho thời gian phản hồi và tần suất, hoặc các điều khiển và hạn chế bảo mật. Một số thông tin này có thể được chỉ định như yêu cầu dữ liệu trong phần 4 hoặc như yêu cầu tương tác trong phần 6, Phẩm chất.  

## **5.3 Hardware interfaces**

Mô tả các đặc điểm của mỗi giao diện giữa các thành phần phần mềm và phần cứng của hệ thống, nếu có. Mô tả này có thể bao gồm các loại thiết bị được hỗ trợ, các tương tác dữ liệu và điều khiển giữa phần mềm và phần cứng, và các giao thức giao tiếp được sử dụng. Liệt kê các đầu vào và đầu ra, định dạng của chúng, các giá trị hoặc phạm vi hợp lệ, và bất kỳ vấn đề thời gian nào mà các nhà phát triển cần biết. Nếu thông tin này rộng rãi, hãy cân nhắc tạo một tài liệu đặc tả giao diện riêng. Để biết thêm về việc đặc tả yêu cầu cho các hệ thống chứa phần cứng."

## **5.4 Communications interfaces**

Nêu các yêu cầu cho bất kỳ chức năng truyền thông nào mà sản phẩm sẽ sử dụng, bao gồm email, trình duyệt web, giao thức mạng, và biểu mẫu điện tử. Định nghĩa bất kỳ định dạng thông điệp liên quan nào. Chỉ định các vấn đề bảo mật và mã hóa truyền thông, tốc độ truyền dữ liệu, bắt tay, và cơ chế đồng bộ. Nêu bất kỳ ràng buộc nào xung quanh các giao diện này, chẳng hạn như liệu một số loại tệp đính kèm email có được chấp nhận hay không.

# **6\. Quality attributes**

Phần này chỉ định các nonfunctional requirement (yêu cầu phi chức năng) ngoài các ràng buộc, được ghi lại trong phần 2.4, và các yêu cầu giao diện bên ngoài, xuất hiện trong phần 5. Những yêu cầu phẩm chất này nên cụ thể, định lượng, và có thể kiểm chứng. Chỉ ra mức độ ưu tiên tương đối của các phẩm chất khác nhau, như dễ sử dụng so với dễ học, hoặc bảo mật so với hiệu suất. Một ký hiệu đặc tả phong phú như Planguage làm rõ mức độ cần thiết của mỗi phẩm chất tốt hơn nhiều so với các tuyên bố mô tả đơn giản.

## **6.1 Tính khả dụng**

Yêu cầu tính khả dụng liên quan đến việc dễ học, dễ sử dụng, tránh và phục hồi lỗi, hiệu quả của các tương tác, và khả năng tiếp cận. Các yêu cầu tính khả dụng được chỉ định ở đây sẽ giúp nhà thiết kế giao diện người dùng tạo ra trải nghiệm người dùng tối ưu.

## **6.2 Hiệu suất**

Nêu các yêu cầu hiệu suất cụ thể cho các hoạt động hệ thống khác nhau. Nếu các functional requirement (yêu cầu chức năng) hoặc tính năng khác nhau có các yêu cầu hiệu suất khác nhau, thì nên chỉ định các mục tiêu hiệu suất đó ngay cùng với các functional requirement (yêu cầu chức năng) tương ứng, thay vì tập hợp chúng trong phần này.  

## **6.3 Bảo mật**

Chỉ định bất kỳ yêu cầu nào liên quan đến các vấn đề bảo mật hoặc quyền riêng tư hạn chế quyền truy cập hoặc sử dụng sản phẩm. Những điều này có thể đề cập đến bảo mật vật lý, dữ liệu, hoặc phần mềm. Yêu cầu bảo mật thường bắt nguồn từ các business rule (quy tắc kinh doanh), vì vậy hãy xác định bất kỳ chính sách hoặc quy định bảo mật hoặc quyền riêng tư nào mà sản phẩm phải tuân thủ. Nếu những điều này được ghi lại trong một kho lưu trữ quy tắc kinh doanh, chỉ cần tham chiếu đến chúng.  

## **6.4 An toàn**

Chỉ định các yêu cầu liên quan đến khả năng mất mát, thiệt hại, hoặc tổn hại có thể xảy ra từ việc sử dụng sản phẩm. Định nghĩa bất kỳ biện pháp bảo vệ hoặc hành động nào phải được thực hiện, cũng như các hành động có khả năng nguy hiểm phải được ngăn chặn. Xác định bất kỳ chứng nhận, chính sách, hoặc quy định an toàn nào mà sản phẩm phải tuân thủ.  

## **\[others\]**

# **7\. Internationalization and localization requirements**

Yêu cầu quốc tế hóa và bản địa hóa đảm bảo rằng sản phẩm sẽ phù hợp để sử dụng ở các quốc gia, văn hóa, và địa điểm địa lý ngoài những nơi nó được tạo ra. Các yêu cầu như vậy có thể giải quyết các khác biệt về tiền tệ; định dạng ngày, số, địa chỉ, và số điện thoại; ngôn ngữ, bao gồm các quy ước chính tả quốc gia trong cùng một ngôn ngữ (như tiếng Anh Mỹ so với tiếng Anh Anh), các ký hiệu được sử dụng, và bộ ký tự; thứ tự tên và họ, múi giờ; các quy định và luật quốc tế; các vấn đề văn hóa và chính trị; kích thước giấy được sử dụng; trọng lượng và số đo; điện áp và hình dạng phích cắm; và nhiều thứ khác. Yêu cầu quốc tế hóa và bản địa hóa có thể được tái sử dụng trên các dự án.  

# **8\. Other requirements**

Định nghĩa bất kỳ yêu cầu nào khác không được đề cập ở nơi khác trong SRS. Ví dụ là các yêu cầu tuân thủ pháp lý, quy định, hoặc tài chính và tiêu chuẩn; yêu cầu cho việc cài đặt, cấu hình, khởi động, và tắt sản phẩm; và các yêu cầu về ghi nhật ký, giám sát, và dấu vết kiểm toán. Thay vì chỉ kết hợp tất cả chúng dưới "Khác", hãy thêm bất kỳ phần mới nào vào mẫu phù hợp với dự án của bạn. Bỏ qua phần này nếu tất cả các yêu cầu của bạn đã được đáp ứng trong các phần khác. Yêu cầu chuyển đổi cần thiết để chuyển đổi từ hệ thống trước sang hệ thống mới có thể được đưa vào đây nếu chúng liên quan đến phần mềm được viết (như cho các chương trình chuyển đổi dữ liệu), hoặc trong kế hoạch quản lý dự án nếu không (như cho việc phát triển hoặc cung cấp đào tạo).  

# **Appendix A: Glossary**

Định nghĩa bất kỳ thuật ngữ chuyên ngành nào mà người đọc cần biết để hiểu SRS, bao gồm các từ viết tắt và chữ viết tắt. Viết rõ từng từ viết tắt và cung cấp định nghĩa của nó. Cân nhắc xây dựng một từ điển thuật ngữ cấp doanh nghiệp có thể tái sử dụng trên nhiều dự án và kết hợp bằng cách tham chiếu bất kỳ thuật ngữ nào liên quan đến dự án này. Mỗi SRS sau đó sẽ chỉ định nghĩa những thuật ngữ cụ thể cho một dự án riêng lẻ không xuất hiện trong từ điển thuật ngữ cấp doanh nghiệp. Lưu ý rằng các định nghĩa dữ liệu thuộc về từ điển dữ liệu, không phải từ điển thuật ngữ.  

# **Appendix B: Analysis models**

Phần tùy chọn này bao gồm hoặc trỏ đến các mô hình phân tích liên quan như sơ đồ luồng dữ liệu, cây tính năng, sơ đồ chuyển đổi trạng thái, hoặc sơ đồ mối quan hệ thực thể. Thường thì việc kết hợp một số mô hình nhất định vào các phần liên quan của đặc tả sẽ hữu ích hơn cho người đọc thay vì tập hợp chúng vào cuối.