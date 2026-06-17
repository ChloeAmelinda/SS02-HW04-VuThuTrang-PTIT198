### **Đáp án: Phương án B**

Phương án B là lựa chọn đúng nhất vì thể hiện đầy đủ trách nhiệm học thuật, tư duy phản biện và vai trò "kiểm duyệt viên" của người học khi sử dụng AI.

AI là công cụ hỗ trợ, không phải nguồn chân lý tuyệt đối. Mặc dù đoạn mã sử dụng `double` có thể hoạt động đúng trong một số trường hợp đơn giản, nhưng đối với các bài toán tài chính, việc sử dụng kiểu dữ liệu dấu phẩy động tiềm ẩn nguy cơ sai số làm tròn. Các sai số nhỏ này có thể tích lũy qua nhiều lần tính lãi kép và dẫn đến kết quả không chính xác.

Người học có trách nhiệm:

* Không tin tưởng hoàn toàn vào kết quả do AI sinh ra.  
* Kiểm tra tính đúng đắn của giải pháp bằng cách đối chiếu với tài liệu chính thức.  
* Hiểu được hạn chế của công nghệ đang sử dụng.  
* Tự xác minh kết quả bằng các trường hợp kiểm thử phù hợp.

Trong Java, giải pháp tiêu chuẩn cho các phép tính tài chính là sử dụng lớp `BigDecimal` kết hợp với `RoundingMode` để kiểm soát độ chính xác và cách làm tròn số. Đây là phương pháp được sử dụng rộng rãi trong các hệ thống ngân hàng, kế toán và thanh toán điện tử.

Ngoài việc yêu cầu AI viết lại hàm bằng `BigDecimal`, sinh viên còn cần tự xây dựng các bộ kiểm thử như:

* Số tiền gửi rất lớn.  
* Lãi suất rất nhỏ.  
* Thời gian gửi kéo dài nhiều năm.  
* Các giá trị biên và trường hợp đặc biệt.

Điều này thể hiện năng lực đánh giá, kiểm chứng và chịu trách nhiệm với sản phẩm do mình nộp, thay vì chỉ sao chép kết quả từ AI.

### **Nhược điểm của phương án A**

Phương án A là hành vi thiếu trách nhiệm học thuật.

Người học sao chép nguyên văn mã nguồn do AI tạo ra chỉ vì chương trình vượt qua một số bộ test đơn giản. Việc một đoạn mã chạy đúng trong vài trường hợp không có nghĩa là nó đúng trong mọi tình huống thực tế.

Các vấn đề của phương án này:

* Tin tưởng tuyệt đối vào AI mà không kiểm chứng.  
* Không xem xét yêu cầu nghiệp vụ tài chính.  
* Không đánh giá rủi ro sai số số học.  
* Không thực hiện kiểm thử bổ sung.

Đây là ví dụ điển hình của việc sử dụng AI một cách thụ động thay vì có tư duy phản biện.

### **Nhược điểm của phương án C**

Phương án C còn kém hơn phương án A.

Việc đổi từ `double` sang `float` không giải quyết được vấn đề mà còn làm giảm độ chính xác tính toán.

Lý do:

* `float` chỉ có khoảng 7 chữ số chính xác.  
* `double` có khoảng 15–16 chữ số chính xác.  
* Cả hai đều sử dụng biểu diễn số thực nhị phân nên đều gặp lỗi làm tròn.

Do đó:

0.1 \+ 0.2

vẫn không được biểu diễn chính xác với `float`.

Phương án này cho thấy:

* Không hiểu bản chất của vấn đề.  
* Không tra cứu tài liệu kỹ thuật.  
* Tự ý chỉnh sửa theo cảm tính.  
* Không đáp ứng tiêu chuẩn xử lý dữ liệu tài chính.

Trong môi trường thực tế, cách làm này có thể dẫn đến sai lệch số tiền và gây hậu quả nghiêm trọng.

### **Kết luận**

**Chọn phương án B.**

Đây là phương án duy nhất thể hiện đúng tinh thần của Lesson 5: sử dụng AI như một công cụ hỗ trợ, nhưng người học vẫn phải giữ vai trò kiểm tra, xác minh, đối chiếu tài liệu chính thức và chịu trách nhiệm cuối cùng về chất lượng của sản phẩm mình nộp. Việc chuyển sang `BigDecimal`, sử dụng `RoundingMode` và tự xây dựng các trường hợp kiểm thử là cách tiếp cận đúng theo cả tiêu chuẩn học thuật lẫn thực tiễn phát triển phần mềm chuyên nghiệp.

