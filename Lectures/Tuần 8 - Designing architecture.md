
---
# Software architecture:

### Definition:

- `Kiến trúc phần mềm sẽ được hiểu theo định nghĩa của Len Bass`

- `Kiến trúc phần mềm:`
	- `Là một tập hợp gồm:`
		- `Tập các "structures", mà trong đó có:`
			- `Software elements.`
			- `Relations among them.`
			- `Properties of both.`
	- `Các loại structures:`
		- `Module Structures.`
			- `Thành phần: [code, classes, packages, layers].`
			- `Mục đích: Source code management, maintenance.`
			- `Các cấu trúc phổ biến:`
				- `Decomposition structure.`
				- `Uses structure.`
				- `Layered structure.`
		- `Component-and-Connector Structures.`
			- `Thành phần: [components, connectors].`
			- `Mục đích: Performance measurement, availability and security check.`
			- `Cấu trúc phổ biến:`
				- `Client-Server.`
				- `Publish-Subscribe.`
				- `Pipe-and-Filter.`
		- `Allocation Structures.`
			- `Thành phần: Môi trường không phải phần mềm (infrastructure, platform, ...).`
			- `Mục đích: Sự phù hợp giữa phần mềm, phần cứng và môi trường vật lí.`
			- ``Các cấu trúc phổ biến:`
				- `Deployment structure.`
				- `Implementation structure.`
				- `Work assignment structure.`
	- `Một số thuộc tính:`
		- `Flexibility: Có thể thay thế được cái khác hay bị thay thế không.`
		- `Portability: Triển khai trên máy khác được không.`
		- `Reusabiliy: Tái sử dụng được không.`
	- `Thuộc tính chất lượng:`
		- `Performance properties:`
			- `Song song hóa.`
			- `Frequency management.`
			- `Giảm nghẽn cổ chai.`
		- `Security properties:`
			- `Authentication and Authorization.`
			- `Layering structure.`
		- `Thuộc tính chung:`
			- `Design qualities.`
			- `Run-time qualities.`
			- `System qualities.`
			- `User qualities.`

# Design architecture:

### Nguyên lí thiết kế:

- `Nguyên lí phân tách:`
	- `Phân ra thành các thành phần càng ít phụ thuộc càng tốt.`
- `Nguyên lí trách nhiệm đơn:`
	- `Chuyên biệt hóa.`
- `Nguyên lí biết tối thiểu:`
	- `Các thành phần biết ít về chức năng của nhau.`
- `Nguyên lí không lặp lại:`
	- `Chức năng được thực hiện bởi chỉ 1 thành phần.`

### Procedure:

- `Xác định mục tiêu.`
- `Xác định hoạt cảnh sử dụng chính:`
	- `Use cases.`
	- `User stories.`
- `Xác định tổng quan ứng dụng:`
	- `Thiết kế khung ứng dụng, design.`
- `Xác định vấn đề phát sinh.`
- `Xác định cách giải quyết vấn đề.`