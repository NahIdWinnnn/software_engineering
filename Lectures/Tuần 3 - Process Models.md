
---
# *Định nghĩa cơ bản:*

### Process (software process):
- `Quá trình tạo ra sản phẩm phần mềm.`
- `Gồm 5 bước: [yêu cầu, thiết kế, cài đặt, kiểm thử, triển khai].`
### Process model:
- `Process là nói chung chung ra gồm 5 bước. Phải có một số "chuẩn" rõ ràng để khoa học, để toán học hơn.`
### Iteration:
- `Mỗi lần làm ra 1 (hoặc một vài) tính năng là một lần phải cập nhật mới vào hệ thống. Mỗi bản vá, bản nâng cấp như thế phải được lên kết hoạch đầy đủ rõ ràng (5 bước chính của process).`
- `Mỗi bản increment đấy chính là một lần lặp. Lặp liên tục, mỗi lần thêm increment vào như một bản nâng cấp, cho đến khi hết vấn đề mới (chính là khi khai tử phần mềm).`

---
# *Một số mô hình quy trình:*

### Waterfall model:

- `Là model đơn giản nhất, đơn giản làm thẳng tuột những gì cần làm là xong phần mềm.`

- `Gồm 5 bước và xác định ngay từ đầu:`
	- `Requirement: Xác định yêu cầu.`
	- `Design: Thiết kế.`
	- `Implementation and testing: Triển khai và thử thử.`
	- `Intergration and testing: Tích hợp và kiểm thử.`
	- `Maintenance: Bảo trì.`

- `Ưu điểm:`
	- `Tài liệu chi tiết đầy đủ`.
	- `Xác định toàn bộ quá trình khi bắt đầu.`
	- `Thích hợp khi làm các dự án cố định, không sai sót, xác định ngay từ đầu.`

- `Nhược điểm:`
	- `Không thể thay đổi nếu đã làm xong.`
	- `Chi phí bảo trì, sửa đổi, nâng cấp rất lớn.`
	- `Vì thiết kế để cuối cùng mới chạy nên sản phẩm sẽ ra mắt hẳn, phiên bản thực có lâu hơn.`
### Evolutionary model:
- `Giống như waterfall model là vẫn gồm 5 bước như trên, nhưng có một số điểm khác biệt:`

	- `Điểm khác biệt là 5 bước này nằm trong 1 vòng lặp.`
	- `Tại bước design, tạo ra một UI để cho người dùng trải nghiệm trước nếu vừa ý thì bắt tay vào làm.`

- `Ưu điểm:`
	- `Sản phẩm đúng ý người dùng.`
	- `Thích ứng nhanh với thay đổi.`
	- `Khách hàng được dùng sớm.`

- `Hạn chế:`
	- `Yêu cầu kĩ năng đặc tả cao.`
	- `Hệ thống có xu hướng bị cấu trúc nghèo nàn, cấu trúc dễ bị nát, cần refactor lại để làm cấu trúc tốt hơn nhưng sẽ vi phạm tam giác ràng buộc.`
### Component-based Software Engineering:
- `Hoạt động trên tư duy module hóa toàn bộ công việc, giống như OOP, mọi thứ đều là một black box hoặc white box.`

- `Cũng gồm 5 bước:`
	- `Requirement: Xác định yêu cầu.`
	- `Component search and evaluate: Xem trên thị trường có những thành phần nào có sẵn.`
	- `Integration design: Thiết kế ra một bản kiến trúc để nối các components.`
	- `Assemble and test: Lắp ráp và kiểm thử.`
	- `Deploy: Triển khai và bàn giao`.
- `Ưu điểm:`
	- `Sản xuất sản phẩm nhanh.`
	- `Tránh rủi ro lỗi sinh ra bởi nghiệp vụ.`
- `Nhược điểm:`
	- `Quá phụ thuộc vào bên thứ 3. Kể cả rủi ro sinh lỗi thì phụ thuộc bên thứ 3.`

### V-model:
- `Một mô hình giống hệt Agile, nhưng một sprint có 5 bước kiểm thử đi kèm đằng sau.`

### Scrum:
- `Một mô hình giống evolutionary development.`
- `Được kế thừa triết lí Agile.`

---

