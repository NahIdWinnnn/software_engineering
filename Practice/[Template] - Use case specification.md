
---
### Template:

```
Use case name: ...
Main actor: ...
Description: ...
Preconditions: ...
Postconditions: ...
Trigger: ...
Scenario: ...
Exception: ...
```

### Illustration:

```
- Use case name: Đăng nhập.
- Main actor: User.
- Description: As a user, I want to đăng nhập, so that tôi có thể sử dụng ứng dụng - theo đúng lợi ích và quyền của mình.
- Preconditions: User đã có tài khoản, vừa mở ứng dụng hoặc vừa đăng xuất.
- Postconditions: User đăng nhập thành công thì vào trang chủ, nếu có lưu session công việc cũ thì phục hồi tiến trình của người dùng.
- Scenario:
  Actor: Vào màn hình đăng nhập.
     System: Hiển thị giao diện đăng nhập.
  Actor: Nhập username, password.
	 System: Kiểm tra format thông tin đăng nhập.
	 System: Xác thực thông tin tài khoản với database.
	 System: Thông báo đăng nhập thành công trong vài giây.
	 System: Ngay sau đó hiển thị ngay giao diện của người dùng.
- Exceptions:
	 System: Thông báo nhập lại vì sai format.
  Actor: Trở lại nhập username, password.
     System: Thông báo nhập lại vì sai email hoặc password và gửi sms nếu có MFA, trở lại giao diện đăng nhập cho actor.
```