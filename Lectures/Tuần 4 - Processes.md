
---
# *Hierarchy:*

- `Các thuật ngữ được chia làm 2 tầng:`
	- `Tầng triết lí:`
		- `Agile: Là triết lí duy nhất của tầng này.`
	- `Tầng process model:`
		- `Process model cổ điển:`
			- `Waterfall.`
			- `V-model (là waterfall model nhưng có 5 bước kiểm thử đối xứng).`
			- `Evolutionary development.`
			- `Component-based.`
			- `RUP: Một process model cũng có nhiều iteration như Scrum, nhưng khổng lồ và rất nặng tài liệu.`
		- `Process model hiện đại:`
			- `Scrum.`
			- `XP.`

# *Các quy trình trọng tâm:*

### Rational Unified Process (RUP):

- `Mô tả về từng luồng hoạt động:`
	- `Inception:`
		- `Đánh giá dự án (theo góc nhìn kinh tế).`
		- `Phác thảo dự án (theo góc nhìn kĩ thuật).`
	- `Elaboration:`
		- `Phát hiện rủi ro.`
		- `Định nghĩa và thiết kế mô hình yêu cầu.`
	- `Construction:`
		- `Casually, phát triển hệ thống.`
	- `Transition:`
		- `Chuyển giao và đảm bảo phát triển tốt trên môi trường khác hàng.`

### Các quy tắc của RUP:

- `Phát triển lặp lại: Tóm lại là có dùng iterations.`
- `Quản lí yêu cầu: Quản lí chặt chẽ bằng use case diagram.`
- `Kiến trúc theo thành phần: Chia làm các modules dễ bảo trì kiểm thử.`
- `Mô hình phần mềm: Sử dụng UML để miêu tả phần mềm.`
- `Liên tục xác minh chất lượng: Đánh giá liên tục qua mọi vòng lặp.`
- `Kiểm soát thay đổi: Dùng công cụ check tầm ảnh hưởng thay đổi.`

---
# *Agile:*

### Triết lí Agile:

- `SRS luôn thay đổi, cần một cấu trúc linh hoạt.`

- `Tiến trình phát triển nhanh:`
	- `Liên tục đặc tả, thiết kế, cài đặt xen kẽ chứ không có một lần chi tiết.`
	- `Tài liệu thiết kế tối giản hoặc tự động.`
	- `Nhiều phiên bản.`
	- `Người dùng và nhà đầu tư cùng tham gia đặc tả và cùng đề xuất (tư vấn).`

- `Incremental development, mỗi lần increment là một lần lặp, mỗi lần lặp gọi là một sprint.`

### Scrum (implements Agile):

- `Thành phần cơ bản của Scrum:`
	- `Roles:`
		- `Scrum master:`
			- `Người này support dev team, xin trợ cấp, tạo điều kiện, giải quyết vấn đề cùng dev team.`
		- `Product owner:`
			- `Người này làm việc và hiểu khách hàng muốn gì, kiểm tra và chỉ đạo dev team làm đúng tiến độ và đúng ý khách hàng.`
		- `Development team.`
	- `Artifacts:`
		- `Product backlog: Danh sách các user stories.`
		- `Sprint backlog: Danh sách vòng lặp.`
		- `Increment: Cái snapshot mới được tạo ra để thêm vào (tưởng tượng nó giống như tạo new version của một persistent segment tree).`
	- `Events (một sprint):`
		- `Spring planning: Họp team chia task.`
		- `Daily Scrum: Họp hàng ngày, kiểm tra phát sinh.`
		- `Sprint review: Khách hàng và project owner kiểm tra.`
		- `Sprint retrospective: Kết thúc sprint.`

- `Bản thân Scrum là liên tục lặp lại sprint cho đến khi xong.`

### Extreme programming (implements Agile):

- `Hoạt động khá giống Scrum.`
- `Điểm lưu ý duy nhất:`
	- `Xử lí một user story.`
	- `Một developer pilot, một developer navigator.`
	- `Test-driven programming, viết test xong mới code một luồng chính thực hiện.`

- `Tính chất nổi bật:`
	- `Pair programming.`
	- `Test-driven programming.`
	- `Tái cấu trúc liên tục: Viết xong test hiệu năng, sau này lại đập đi làm lại để tích hợp tốt hơn, tối ưu hơn nữa.`

### Khi nào nên sử dụng, khi nào nên tránh:

- `RUP:`
	- `Nên dùng khi:`
		- `Quy mô cực lớn.`
		- `Kiến trúc lõi rất quan trọng.`
		- `Development team đông hoặc phân tán.`
		- `Yêu cầu về tài liệu rất khắt khe.`
	- `Không nên khi:`
		- `Quy mô nhỏ, vừa.`
		- `Time to market ngắn, cần gấp.`
		- `Yêu cầu thay đổi linh hoạt.`

- `Scrum:`
	- `Nên dùng khi:`
		- `SRS mơ hồ.`
		- `Dự án quy mô vừa, nhỏ, hoặc có thể chia nhỏ.`
		- `Time to market ngắn.`
		- `Quản lí dev team tốt.`
	- `Không nên khi:`
		- `Hệ thống yêu cầu an toàn.`
		- `Hệ thống nặng tài liệu và chốt cứng tính năng.`
		- `Khách hàng khó hợp tác.`

- `XP:`
	- `Nên dùng khi:`
		- `Yêu cầu thay đổi nhiều.`
		- `Dự án cần chất lượng rất cao.`
		- `Cần dev team phối hợp tốt và khách hàng phối hợp.`
	- `Không nên khi:`
		- `Dev team quản lí không tốt.`
		- `Dự án lớn.`
		- `Quy mô dự án lớn.`

---
