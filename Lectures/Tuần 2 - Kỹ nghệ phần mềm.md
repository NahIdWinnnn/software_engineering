
---
# *Khái niệm Software Engineering*
### Software Engineering:
- `Bản chất: Là một ngành công nghiệp.`
- `Cách thức: Sử dụng mọi khía cạnh khoa học công nghệ.`
- `Mục đích: Phát triển phần mềm một cách "hiệu quả", "kinh tế".`

### Kỹ nghệ:
- `Bản chất: "Kỹ thuật" và "công nghệ" xây dựng phần mềm.`
- `Cách thức: Sử dụng mọi lí thuyết, phương pháp, công cụ.`
- `Mục tiêu: Tạo ra giải pháp, kể cả khi không có sẵn tools hoặc theory.`

### Yêu cầu:

- **`1. Chất lượng cao:`**
	- `reliability.`
	- `performance efficiency.`
	- `maintainability.`
	- `security.`
	- `usability.`
	- `portable.`

- **`2. Thời gian phát triển ngắn:`**
	- `development time.`
	- `delivery schedule.`

- **`3. Chi phí phát triển thấp`**
	- `development cost.`
	- `maintenance cost.`

---
# *Các thành phần của Software Engineering*

### Tổng hợp thành phần:

- **`1. Process model:`**
	- `Prerequisite: Nhằm mục đích cho một sản phẩm chất lượng cao.`
	- `Bản chất: Thứ tự, các bước, giai đoạn, mô hình quản lí con người khi làm một dự án.`
	- `Một số mô hình: Waterfall model, Spiral model, Incremental model, Agile process.`
	- `Accompanied resource: Tài liệu, sản phẩm, cách thức thực hiện.`
	- `Xác định rõ các mốc thời gian.`

- **2. Methods:**
	- `Prerequisite: Khi đã xác định các giai đoạn, các bước dự án tại "process model".`
	- `Bản chất: Quy định và cách thức để làm những công đoạn đó.`
	- `Mỗi giai đoạn:`
		- `1. Phân tích (thu thập, phân tích, đặc tả yêu cầu).`
		- `2. Thiết kế (kiến trúc, giao diện, dữ liệu, database).`
		- `3. Lập trình (cấu trúc, hướng đối tượng).`
		- `4. Kiểm thử (hộp đen, hộp trắng, hồi quy).`
		- `5. Quản lý dự án (PERT, COCOMO).`

- **`3. Tools:`**
	- `Prerequisite: Sau khi xác định được các methods được sử dụng cho từng giai đoạn.`
	- `Bản chất: Cụ thể hóa công cụ được lắp vào các methods được thiết kế ra.`
	- `Trong SE, các công cụ nói chung được gọi là CASE tools: Hỗ trợ nhiều hoạt động phát triển phần mềm như "phân tích, thiết kế, lập trình, kiểm thử, quản lí dự án".`
	- `Công dụng: Tự động hóa và giảm thủ công, giảm sai sót, tăng năng suất.`

---
# *Đặc thù & Sự tiến hóa của Software Engineering*

### Phân biệt vai trò:

**`1. Nhà khoa học:`**
- `Nhiệm vụ: Nghiên cứu, đề xuất các giải pháp, phương pháp và công cụ mới.`
- `Nguồn lực: Có thời gian vô hạn.`

**`2. Kỹ sư phần mềm:`**
- `Nhiệm vụ: Phát triển giải pháp thực tế cho một vấn đề cụ thể, phục vụ tệp khách hàng cụ thể.`
- `Môi trường: Làm việc trên nhiều miền ứng dụng khác nhau, luôn đối mặt với môi trường biến động liên tục.`
- `Ràng buộc: Có thời hạn (deadline) làm việc nghiêm ngặt và phải dùng ngôn ngữ, công cụ, kỹ thuật cụ thể.`

---
# *Vòng đời & Khủng hoảng phần mềm*

### Vòng đời phát triển (SDLC):
- `Bản chất: Toàn bộ hoạt động từ khi được đặt hàng, phát triển, sử dụng cho đến khi bị loại bỏ.`
- `Các pha chính:`
    - `1. Lập kế hoạch: Thu thập sơ bộ, ước lượng sớm và lập kế hoạch.`
    - `2. Phân tích & Đặc tả: Thu thập, phân tích, viết đặc tả và thẩm định yêu cầu.`
    - `3. Phát triển: Thiết kế -> Triển khai (Lập trình) -> Kiểm thử -> Viết tài liệu.`
    - `4. Tiến hóa (Bảo trì): Vận hành, sửa lỗi, làm thích nghi, bổ sung và nâng cấp.`

---
# *Phân bổ chi phí & Đạo đức nghề nghiệp*

### Chi phí phát triển (Cost Distribution):
- `Bản chất: Chi phí phát triển ban đầu chỉ là "phần nổi của tảng băng chìm". Gánh nặng thực sự nằm ở quá trình **Bảo trì kéo dài**.`
- `Ước lượng tỷ lệ phân bổ chi phí chuẩn:`
    - `Xác định yêu cầu & Đặc tả: ~ 6% (3% + 3%)`
    - `Thiết kế: ~ 5%`
    - `Lập trình: ~ 7%`
    - `Kiểm thử: ~ 15% (Mô-đun 8% + Tích hợp 7%)`
    - `Bảo trì & Vận hành: ~ 67% (Chiếm áp đảo)`

### Đạo đức nghề nghiệp (Professional Ethics):
- `Yêu cầu bắt buộc: Đảm bảo tính chuyên nghiệp.`
- `Tuân thủ: Thực hiện nghiêm túc quy tắc đạo đức, ứng xử nghề nghiệp và các vấn đề về luật pháp liên quan đến bản quyền, dữ liệu.`

---
