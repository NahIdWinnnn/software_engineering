
---
### Verification and Validation:

- `Verification: Kiểm chứng.`
	- `Kiểm tra sản phẩm có đúng như thiết kế không?`
- `Validation: Thẩm định.`
	- `Kiểm tra sản phẩm có đáp ứng nhu cầu khách hàng?`

- `Static "V&V":`
	- `Đặc điểm: Không chạy code.`
	- `Kiểm tra bằng review, tiến hành ở mọi giai đoạn, xét duyệt yêu cầu.`
	- `Đối tượng kiểm tra: Source code, SRS, tài liệu thiết kế, architecture.`
- `Dynamic "V&V":`
	- `Đặc điểm: Thực thi code.`
	- `Là cách duy nhất thực hiện các yêu cầu phi chức năng.`
	- `Đối tượng kiểm tra: Compiled source code.`
	- `Phương tiện: testcase (gồm input, steps, expected output).`

### Quality and Reliability:

- `Quality:`
	- `Chất lượng: Sự thỏa mãn sản phẩm so với đặc tả.`
	- `Thuộc tính của chất lượng: [6 thuộc tính chất lượng trong bài 2].`

- `Reliability:`
	- `Tin cậy: Độ bền, ổn định của sản phẩm trong một khoảng thời gian và môi trường.`
	- `Các thuộc tính của tin cậy:`
		- `High availability.`
		- `Tính xác suất số lần chạy lỗi trong tổng số lần chạy.`

### Thông tin chung về testing:

- `Testable code:`
	- `Là code theo kiểu có thể "dùng code khác" để check lại chính nó.`
	- `Ví dụ như có một số hàm builtin khó mà viết code check được vì nó khá rigid.`
- `Test-driven development:`
	- `Viết testcases trước rồi từ đó phát triển ra implementation.`
	- `Có thể áp dụng vào Scrum hoặc mô hình tiến hóa.`

- `Micro skill - testing một cơ chế:`
	- `Truy vấn.`
	- `Unit test.`
	- `Gián tiếp bằng đăng nhập.`

- `Độ nghiêm trọng:`
	- `High (10): Tính năng không hoạt động.`
	- `Medium (2 hoặc 3): Tính năng hoạt động không hoàn chỉnh (và có cách chống chế tạm thời).`
	- `Low (1): Lỗi nhỏ không ảnh hưởng chức năng hệ thống.`

- `Loại lỗi:`
	- `Internal (lỗi trong): Lỗi được phát hiện trong kiểm thử nội bộ trước khi sản phẩm được bàn giao hoặc release`
	- `External (lỗi ngoài) (aka "leakage"): Lỗi còn lại phát hiện bởi khách hàng và người dùng cuối.`

- `Norm: Chuẩn thống kê theo các công ty.`
	- `Số bug / size dự án (side dự án tính bằng man-month).`
	- `Độ nghiêm trọng.`
	- `Lấy trọng số [1, 2, 10] cho độ nghiêm trọng chia trung bình man-month.`

### Hoạt động kiểm thử:

- `Hoạt động kiểm thử chia làm 5 bước tương ứng với đúng 5 bước trong một mô hình tiến trình:`
	- `Requirements (yêu cầu): Test condition - xác định xem những gì cần test.`
	- `Design (thiết kế): Test design - cách để test.`
	- `Implementation (xây dựng): Create testcases - tạo testcases.`
	- `Testing (kiểm thử chính): Test execution - thực thi testcases.`
	- `Maintainment (vận hành): Evaluation - đánh giá so với "expected output".`

- `Testcase: Gồm các tính sau.`
	- `Gồm 3 yếu tố: "Input", "Steps" và "Expected output".`
	- `Trình bày:`
		- `Metadata: Tên tính năng, người viết testcase, tiền điều kiện, người test.`
		- `Report: Tổng, số testcases accepted và failed, not applicable, thống kê bug 3 loại.`
		- `Kịch bản kiểm thử chi tiết: Bảng bên dưới.`

| Thứ tự | Các bước KT (Test Steps)                                                                                                                                                                        | Expected result (Kết quả mong đợi)   | Actual result (Kết quả thực tế) | BugID | Version |   Status   |
| :----: | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :----------------------------------- | :------------------------------ | :---: | :-----: | :--------: |
| **1.** | **Điều kiện:** <br>- Username: `vietth` đã có trong database.<br>- Password: `123456`.<br><br>**Các bước thực hiện:**<br>- Nhập username: `vietth`.<br>- Nhập password: `123`.<br>- Nhấn login. | - Không login được. <br>- Báo lỗi... | - Login thành công.             | BG56  |  1.0.1  | **Failed** |

#### Hướng tiếp cận kiểm thử:
- `Bộ testcase tốt:`
	- `Đặt P là một chương trình, S là một đặc tả, T là một bộ testcase.`
	- `Là một bộ phủ được bao nhiêu % chức năng, yêu cầu của S.`

- `Kiểm thử hộp đen:`
	- `Tính chất và cách hoạt động:`
		- `Do nó là black box, chúng ta chỉ có thể test behavior của nó.`
		- `Vì thế, chúng ta phải test trên input.`
		- `Nhưng test input thì phải dựa trên SRS.`
		- `Tiêu chí phủ trong mô hình P, S, T ...`
		- `Vì nó là hộp đen nên nó độc lập với code.`
	- `Mục tiêu: Giảm số lượng ca kiểm thử bằng cách chia không gian nghiệm.`

- `Kiểm thử hộp trắng:`
	- `Tính chất và cách hoạt động:`
		- `Do hiểu bản chất, có thể mô hình hóa tư duy.`
		- `Điển hình là CFG/DFG là 2 loại đồ thị hay dùng cho mô hình tư duy.`
		- `Đặt ra tiêu chí độ phủ dựa trên graph theory.`
		- `Suy ra có thể độ phủ chính là độ phủ trên tất cả các đường đi trên mô hình tư duy này, mỗi đường đi tổng với nhau là đồ thị DAG.`

- `So sánh:`
	- `Kiểm thử hộp trắng không hợp với hệ thống và hệ thống tích hợp vì có quá nhiều đường đi trên mô hình tư duy.`
	- `Kiểm thử hộp đen dễ bùng nổ về số ca kiểm thử. Khó để phát hiện lỗi cụ thể.`

#### Kiểm thử gỡ lỗi:

- `Các mức kiểm thử nội bộ:`
	- `Kiểm thử đơn vị: Từng phần nhỏ một.`
	- `Kiểm thử tích hợp: Ghép các đơn vị lại.`
	- `Kiểm thử hệ thống: Kiểm thử cả luồng nghiệp vụ chứ không chỉ một tính năng tích hợp như kiểm thử tích hợp. Thậm chí có thể kiểm thử hệ thống như một kernel agent, đánh giá chất lượng (các tính chất như trên) và kiểm thử như thường.`

- `Các mức kiểm thử bàn giao:`
	- `Kiểm thử chất lượng: Kiểm thử phía phát triển.`
	- `Kiểm thử chấp thuận: Kiểm thử phía khách hàng.`
		- `Có hai kiểu kiểm thử chấp thuận:`
			- `BAT: Kiểm thử phía cơ quan phát triển (ví dụ như nhà phát hành game check xem game đủ điều kiện không thì mới chịu phát hành nội địa).`
			- `UAT: Kiểm thử phía người dùng (ví dụ như alpha test, beta test).`
	- `Kiểm thử cài đặt: Kiểm thử phía người dùng.`
+
- `Kiểm thử hồi quy:`
	- `Khi hệ thống chỉnh sửa, cần chạy lại toàn bộ bộ kiểm thử (giống như O(n^2)).`

---
