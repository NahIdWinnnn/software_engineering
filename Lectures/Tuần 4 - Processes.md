
---
# *Nội Dung:*

- `RUP`
- `Agile/XP, Scrum`

---
# *RUP:*

### Rational Unified Process:
- `Gồm 4 pha:`
	- `Inception (specification): Định nghĩa phạm vi dự án.`
		- `Tưởng tượng như giám đốc dự án nghĩ có nên làm không một project, nhỡ nó flop, nhỡ nó không thực dụng hay vô nghĩa, nhớ nó lỗ.`
		- `Xác định phạm vi xem dự án này to hay nhỏ để triển khai nhân lực và đánh giá tài chính.`
		- `Nhận diện use-case chính (20%).`
	- `Elaboration (design): Lập kế hoạch, đặc tả kiến trúc cơ bản.`
		- `Brainstorm để tìm ra cấu trúc cốt lõi, khung xương dự án.`
		- `Do đó, đây là bước hoàn thành nốt use-case (80%).`
		- `Có một chút implementation ở đây, tạo ra khung có thể dùng được trước được để chứng minh và sau đó kiểm thử.`
	- `Construction (implementation): Phát triển phần mềm.`
		- `Phát triển song song các phần của hệ thống, gồm nhiều lập trình viên.`
	- `Transition (deploy): Bàn giao cho người dùng.`
		- `Bàn giao và đảm bảo hoạt động tốt trong môi trường người dùng.`

- `RUP rất gần với Waterfall model, tưởng tượng chính RUP là một cái modified waterfall để dành cho metadata, scope dự án. Đến bước 3 (construction) mới là làm thật. Bên trong bước này lại là lặp lại nhiều lần quy trình 5 bước của Waterfall.`

### Business Process Modeling Notation:
- `Trước khi đi vào mô hình, cần biết trước cách vận hành của khách hàng. Sinh ra BPMN để biết khách hàng đặt phần mềm hoạt động thế nào để viết ra phần mềm.`
- `BPMN có thể coi như một phần của Inception, hoặc thậm chí là trước Inception.`
- `Được nghiên cứu bởi giám đốc, BA (Business Analyst).`

### 6 quy tắc của RUP:
- `Phát triển lặp lại: Từng bước được lặp lại nhiều lần.`
- `Quản lí yêu cầu:`
	- `Tài liệu thay đổi yêu cầu.`
	- `Ảnh hưởng của yêu cầu lên toàn bộ phạm vi.`
	- `Lưu vết thay đổi.`
- `Sử dụng kiến trúc dựa trên từng thành phần.`
- `Mô hình phần mềm trực qua: Có thể dùng UML.`
- `Kiểm chứng chất lượng phần mềm.`
- `Kiểm soát thay đổi phần mềm.`

---
# *Agile/Scrum:*

### Agile:
- `Một bộ quy tắc thực hành cho phát triển phần mềm. Tóm lại là lí thuyết, triết học, giống như một interface trong Java.`
- `Scrum, XP, ... là các processes dựa trên agile, là class implements agile.`

### Triết lí Agile:
- `Một tập yêu cầu cố định là không thể, yêu cầu ban đầu luôn thay đổi, cần một cách triển khai dự án robust với sự thay đổi liên tục này.`
- `Hậu quả của việc thay đổi là không cần bàn cãi.`
- `Tiến trình phát triển nhanh:`
	- `Liên tục đặc tả, thiết kế, cài đặt xen kẽ chứ không có một lần chi tiết.`
	- `Tài liệu thiết kế tối giản hoặc tự động.`
	- `Nhiều phiên bản.`
	- `Người dùng và nhà đầu tư cùng tham gia đặc tả và cùng đề xuất (tư vấn).`
- `Incremental development, mỗi lần increment là một lần lặp, mỗi lần lặp gọi là một sprint.`

### Scrum (implements Agile):
- `Một framework để team quản lí công việc.`
	- `Các vai trò:`
		- `Scrum master.`
		- `Product owner.`
		- `Development Team.`
	- `Các tài liệu:`
		- `Product backlog: Viết dưới dạng User Story.`
		- `Sprint backlog.`
		- `Product increment: phần snapshot mới của phần mềm sau một sprint.`
	- `Trong một sprint có 4 bước:`
		- `Sprint planning: Họp team để lấy task.`
		- `Daily Scrum: Kiểm tra có khó khăn bất ngờ xảy ra không.`
		- `Sprint review: Khách hàng và project owner đến kiểm tra.`
		- `Sprint retrospective: Kết thúc sprint.`

### Extreme programming (implements Agile):
- `Pair programming.`
- `Test-driven programming.`
- `Tái cấu trúc liên tục: Viết xong test hiệu năng, sau này lại đập đi làm lại để tích hợp tốt hơn, tối ưu hơn nữa.`

### Một số tool hay dùng để quản lí backlog và sprint:
- `Jira.`
- `Trello.`
- `Asana.`

---
