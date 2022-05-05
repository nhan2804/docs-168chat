# Dự án ( Application)

## Tạo tự án

`Dự án` -> `Tạo mới dự án`

### Cấu trúc

- `Logo` : Logo của dự án (optional)
- `Tên App` : Tên của dự án
- `Miêu tả` : Miêu tả về dự án
- `URL Web` : Url web của trang web bạn muốn nhúng 168chat, nếu nhập sai, 168chat sẽ báo lỗi v. Ví dụ : `https://soundcloud.com/`,`https://serpapi.com/`

## Cấu hình dự án

`Dự án` -> `Danh sách dự án` -> `Cấu hình`

### Cấu hình giao diện

- Câu thông báo chào
- Miêu tả chào
- Màu sắc : Màu sắc chủ đạo sẽ xuất hiện của iframe 168chat
- Background : Hình nền ở đầu khung chat
- Custom Button : Hình của nút bấm để hiển thị ra 168chat
- Vị trí hiện Popup
- Thêm input trước khi chat : Khi bạn muốn khách hàng điền những thông tin trước khi chat (Những thông tin được điền sẽ được hiển thị bên trong cửa sổ chat : Hover vào biểu tượng `Window,Android,Web`để xem)`e.g`

```json
[
  {
    "type": "input",
    "label": "Họ và tên",
    "name": "name",
    "placeholder": "Nhập họ và tên",
    "rules": [{ "required": "true", "message": "Vui lòng nhập họ và tên!" }]
  },
  {
    "type": "input",
    "label": "Vấn đề gặp phải",
    "name": "problem",
    "placeholder": "Nhập vấn đề bạn gặp phải",
    "rules": [
      { "required": "true", "message": "Vui lòng nhập vấn đề của bạn!" }
    ]
  }
]
```

### Cấu hình nâng cao

- Cấu hình cuộc gọi :
- - `Cho phép gọi ( audio/video )` : Cho phép các Customer Service có thể gọi điện cho khách hàng, có thể cài đặt riêng trong phần cấu hình từng thành viên
- - `Số lượng mỗi CS được phép nhận cuộc gọi` : Số lượng mỗi CS có thể nhận các cuộc chat đồng thời từ khách hàng
- - `Chat trên các nền tảng khác` : Tính năng cho phép khách hàng có thể chat trên các nền tảng khác ( Khi Customer Service cập nhật thông tin)
- Âm thanh, thông báo : Bật/Tắt những âm thanh
  > Thử tạo 1 dự án và thử ngay
