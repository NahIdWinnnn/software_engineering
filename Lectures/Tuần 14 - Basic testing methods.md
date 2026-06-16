
---
# Boundary Value Analysis:

### Context:
- `Coi chương trình là một hàm toán học.`
	- `Input: Đầu vào là miền xác định của hàm.`
	- `Output: Đầu ra là miền giá trị của hàm.`
- `Phân tích giá trị biên (BVA):`
	- `Là một kĩ thuật kiểm thử hàm phổ biến.`
- `Mô hình tư duy:`
	- `Coi chương trình là một hàm thì bản thân nó giống một set trên biểu đồ Venn.`
	- `Biểu đồ Venn: Chia làm nhiều phần, trong đó có các vibe như, 2 thằng cùng 1 miền thì "hành vi" hệ thống lên chúng giống nhau, tất nhiên là output khác nhau nhưng xu hướng, vibe, aura, giống nhau.`
	- `Mô hình hóa thế này có thể rời rạc hóa được chương trình.`
	- `Nhưng ở biên thì thường có nhiều edge cases.`

### Boundary Value Analysis (BVA):
- `Mô hình tư duy:`
	- `Tưởng tượng không gian nghiệm của một số hệ phương trình, chính là các biến độc lập tại input chương trình trên tập xác định.`
- ***`Cách chọn các giá trị biên kiểm thử:`***
	- `Min: Giá trị nhỏ nhất trong miền.`
	- `Min+: Giá trị nhỏ nhì trong miền, tăng lên một chút.`
	- `Mean: Giá trị bất kì nằm giữa, hoặc là trung bình min và max.`
	- `Max-: Giá trị lớn nhất trong miền giảm đi một chút.`
	- `Max: Giá trị lớn nhất.`

### Giả thuyết khiếm khuyết đơn:

### Tổng quát hóa:
- `Có 2 cách tổng quát hóa:`
	- `Cách 1: Theo số biến, tính (4n + 1) ca kiểm thử cho n biến.`
		- `Điều kiện: Cần có giả thuyết khiếm khuyết đơn.`
	- `Cách 2: Theo loại khoảng của biên.`
		- `Ví dụ như theo ngôn ngữ lập trình, theo tính rời rạc, theo rời rạc không bị chặn, biến logic.`
### Kiểm thử biên mạnh và trường hợp xấu nhất:
- `Kiểm thử biên mạnh:`
	- `Bổ sung thêm min- và max+.`
- `Kiểm thử trường hợp xấu nhất:`
	- `Bỏ đi giả thuyết khiếm khuyết đơn.`
	- `Có thể kiểm tra nhiều biến tại min, max cùng lúc.`
- `Kiểm thử trường hợp xấu nhất mạnh:`
	- `Vừa kiểm thử nhiều biến tại min, max.`
	- `Vừa bổ sung min- và max+.`

# Equivalence Partitioning:

### Context:
- `Kỹ thuật kiểm thử hộp đen.`
- `Phân miền dữ liệu vào nhiều partitions, mỗi vùng có hành vi xử lí giống nhau.`

### Equivalence Class Testing:

- `Quy tắc cơ bản:`
	- `Phân loại vùng tương đương:`
		- `Phân vùng hợp lệ.`
		- `Phân vùng không hợp lệ.`
	- `Quy tắc xác định lớp tương đương đầy đủ:`
			- `Điều kiện là range:`
				- `Xác định 1 lớp hợp lệ và 2 lớp không hợp lệ.`
			- `Điều kiện là specific value:`
				- `Xác định 1 lớp hợp lệ và 2 lớp không hợp lệ.`
			- `Điều kiện là một member of a set:`
				- `Xác định 1 lớp hợp lệ và 1 lớp không hợp lệ.`
			- `Điều kiện là một boolean:`
				- `Xác định 1 lớp hợp lệ và 1 lớp không hợp lệ.`

- `Kiểm thử lớp tương đương yếu, mạnh, đầy đủ:`
	- `ECT yếu:`
		- `Đảm bảo mỗi lớp tương đương xuất hiện ít nhất 1 lần.`
	- `ECT mạnh:`
		- `Yêu cầu phủ tất cả tổ hợp của các lớp tương đương (tích đề các).`

# *Decision Table:*

### Properties:
- `Representation: Biểu diễn "yêu cầu chức năng" bằng Decision Table.`
- `Capability: Có khả năng liên kết "nhiều điều kiện độc lập" với "nhiều hành động" một cách dễ hiểu.`

### Structure: ...

---
