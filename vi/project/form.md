# Form

## Tạo form

`Dự án` -> `Form` -> `Tạo mới form`

### Cấu trúc

- `Tên form` : Tên của form
- `Nội dung` : Nội dung của form phải là json và phải đúng format
- `e.g` :

```json
[
  {
    "type": "input",
    "label": "Họ và tên",
    "name": "name",
    "placeholder": "Nhập họ và tên"
  },
  {
    "type": "input",
    "label": "Phone",
    "name": "phone",
    "placeholder": "Nhập SDT"
  },
  {
    "type": "image",
    "label": "Ảnh CMND",
    "name": "cmnd",
    "placeholder": "Chọn CMND"
  },
  {
    "type": "date",
    "label": "Ngày hết hạn",
    "name": "exprired",
    "placeholder": "Chọn ngày"
  },
  {
    "type": "select",
    "label": "Khu vực",
    "name": "region",
    "placeholder": "Chọn khu vực",
    "options": [
      {
        "name": "Miền Bắc",
        "value": "mb"
      },
      {
        "name": "Miền Trung",
        "value": "mt"
      },
      { "name": "Miền Nam", "value": "mn" }
    ]
  },
  {
    "type": "radio",
    "label": "Giới tính",
    "placeholder": "Chọn giới tính",
    "name": "gender",
    "options": [
      {
        "name": "Nam",
        "value": "n"
      },
      {
        "name": "Nữ",
        "value": "nu"
      },
      { "name": "????", "value": "dd" }
    ]
  },
  {
    "type": "checkbox",
    "label": "Sở thích",
    "name": "hobby",
    "placeholder": "Chọn sở thích",
    "options": [
      {
        "name": "Nghe nhạc",
        "value": "x"
      },
      {
        "name": "Code",
        "value": "y"
      },
      { "name": "Fix bug", "value": "z" }
    ]
  },
  {
    "type": "single-checkbox",
    "label": "Xac Nhan",
    "name": "verify",
    "placeholder": "Chọn xc nhan"
  }
]
```

## Cách dùng form

- Chọn vào biểu tượng form
- ![Tạo form](https://i.ibb.co/0hH8Fp5/image.png)
- Chọn form cần gửi cho khách hàng
- Đợi phản hồi của khách hàng
- ![Form phản hồi](https://i.ibb.co/mbCY1J4/image.png)
- Bấm vào `Xem` để xem form, bấm vào `icon 3 chấm` để Yêu cầu nhập lại, hủy form hoặc lưu
- Đối với lưu form, bạn cần nhập miêu tả form , và các tags cần thiết để sau này tìm lại cho dễ
- Nếu form có chứa hình ảnh, vui lòng nhập miêu tả và tags như form

## Tính năng thêm

- Sau khi lưu form của khách, mỗi khi bạn nhắn tin mà có chứa từ khóa liên quan đến form bạn đã lưu của khách hàng đó, hệ thống sẽ tự động recomment cho bạn lại form,hình ảnh đã lưu
- Kho data cũng sẽ lưu tất cả form data mà bạn đã lưu ( Ref )
  > Thử tạo 1 form và thử ngay
