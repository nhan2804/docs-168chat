# Form

## Tạo form

`Dự án` -> `Form` -> `Tạo mới form`

### Cấu trúc

`Tên form` : Tên của form
`Nội dung` : Nội dung của form phải là json và phải đúng format
`e.g` :

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

### Import package 168chat

Ở file `./App.js` import package react- 168chat.

```js
<!-- ./App.js -->
import React168Chat from "react-168chat"

<React168Chat
  projectId="9283239339933"
  secret="ndfnfdfdfndkndfn"
  extras="{}"
></React168Chat>
```

## ReactNative

```bash
npm i react-native-168chat
```

### Import package react-native-168chat

Ở file `./App.js` import package 168chat.

```js
<!-- ./App.js -->
import RN168Chat from "react-native-168chat"

<RN168Chat
  projectId="9283239339933"
  secret="ndfnfdfdfndkndfn"
  extras="{}"
  onClose={}
  isVisiable={true}
></RN168Chat>
```

## Cocos Creator

### Import package react-native-168chat

```js
<!-- ./App.js -->
let coming = "soon"

```

> Các thông tin được tìm thấy ở dashboard 168chat.com/.
