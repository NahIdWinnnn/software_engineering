
---
### Functional Requirements:

```
Requirement ID: ...
Name: ...
Description: ...
Inputs: ...
Processing: ...
Outputs: ...
Exceptions: ...
Priority: ...
```

### FR Illustration:

```
ID: "FR-ORDER-015"
Name: Tính chiếu khấu đơn hàng.
Description: Hệ thống tự động áp dụng chiết khấu cho tổng đơn hàng, dựa vào cấp độ thành viên của khách hàng.
Inputs: Tổng giá trị đơn hàng, cấp độ thành viên khách hàng.
Processing:
	- Hạng Đồng: chiếu khấu 0%.
	- Hạng Bạc: chiết khấu 5%.
	- Hạng Vàng: chiết khấu 10%.
Outputs: Giá tiền cuối cùng theo VNĐ, số tiền đã chiết khấu.
Exceptions: Nếu không có thông tin cấp độ thành viên, sử dụng mặc định 0% chiết khấu.
Priority: Cao.
```

### Non-Functional Requirements:

```
Requirement ID: ...
Categories: [Performance (Efficiency), Reliability (Security), Usability, Portable, Maintainability].
Name: ...
Description: ...
Measure: ...
Acceptance Criteria: ...
```

### NFR Illustration:

```
ID: NFR-PERF-009
Categories: Performance.
Name: Thời gian phản hồi tìm kiếm sản phẩm.
Description: Khi người dùng bấm nút tìm kiếm sản phẩm, hệ thống phải trả về kết quả trong thời gian quy định.
Measure: Tính bằng giây.
Acceptance Criteria: Trung bình kì vọng 1s cho 95% truy vấn với bối cảnh 1000 ngươì truy cập đồng thời. 
```