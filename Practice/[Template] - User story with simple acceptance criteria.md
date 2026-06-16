
---
### Template:

```
[user story]:
As a <role>, I want to <action> so that <benefit>

[acceptance criteria]:
- Condition 1.
- Condition 2.
- Condition 3.
...
```

### Illustration:

```
Illustration 1:

- Context: Đang xây dựng ứng dụng đặt đồ ăn trực tuyến.

User story:
	As a khách hàng thường xuyên của ứng dụng, 
	I want to lưu lại các địa chỉ giao thàng thường xuyên tôi hay dùng, 
	So that tôi cảm thấy tiện lợi hơn khi đặt hàng, không rườm rà.

Acceptance Criteria:
	- Tại màn hình nhập địa chỉ lần đầu, có nút "lưu địa chỉ cho lần sau".
	- Người dùng có thể đặt tên gợi nhớ cho địa chỉ này khi bấm vào nút lưu.
	- Hệ thống cho phép tối đa 10 địa chỉ khác nhau.
	- Người dùng vào setting hoặc giao diện chính của ứng dụng để chỉnh danh sách.
	- Danh sách địa điểm đã lưu hiện ra tại màn hình chính, hoặc trên thanh search.
	- Dach sách địa điểm cả 2 trường hợp đều là dạng bảng, xếp theo thiờ gian gần nhất của mỗi địa điểm.
```

```
Illustration 2:

- Context: Đang xây dựng ứng dụng quản lí tài khoản ngân hàng cá nhân.

User story:
	As a khách hàng của ứng dụng,
	I want to xem được các thông báo về các khoản tiền cần trả online,
	So that tôi có thể đảm bảo bills được trả đúng hạn.

Acceptance Criteria
	- Thông báo về các khoản thanh toán hiện ngay ở màn hình chính.
	- Được thiết kế theo dạng danh sách từ trên xuống.
	- Được sắp xếp theo thứ tự thời gian cần trả từ sớm nhất trở đi.
	- Có tag phân loại rõ ràng là "quá hạn", "cận kề", "tương lai".
	- Có đầy đủ thông tin như người thanh toán, thời gian, khoản tiền.
```

### Thông tin bổ sung:

- `Acceptance criteria được phê duyệt bởi Product Owner.`