# Server side rendering

## Paste Script vào file bạn muốn hiển thị livechat

Ví dụ index.html

```html
<!--
    // index.html
<script data-src-embed="https://embed.168chat.com/" data-src-js-embed="https://168chat.com/" id="embed-live168" data-id=626766b142e5bcee11562a00 src="https://168chat.com/embed/template/index.js"></script>

<script>
    //Truyền các thông số cần thiết
    window.Live168API.init({
      webId: "626766b142e5bcee11562a00",
      extras: {
        userId:"User id",
        vToken:" v token ",
        fullname: "Name of user",
        age: 21,
        more: "more and more",
      },
    });
</script>
```

Trong đó

- `extras.userId` : Nếu bạn muốn xác thực người dùng, vui lòng truyền userId vào
- `extras.vToken` : Để xác thực được userId, bạn cần phải gọi http request qua 168chat để có thể lấy được vToken

## Các bước để xác thực người dùng

- Truy cập vào trang cấu hình dự án
- ![Truy cập vào trang cấu hình dự án](https://i.ibb.co/FhsfQFf/image.png)
- Ở `Cấu hình xác minh`, nếu chưa có token, hãy bấm vào `Tạo mới` và copy token
- Sau khi lấy được token, ở phía máy chủ bạn trước khi render ra html, bạn sẽ phải gọi 1 http request qua 168chat
- [`POST`]`https://168chat.com/api/projects/{projectId}/verify-token/encode`
- [`BODY`]

```json
{
  "payload": {
    "userId": "user id" // optional
  },
  "verifyToken": "SxrkakWxg8vbhEVylHBx2" // ở đây là token đã copy lúc nãy
}
```

- 168chat sẽ return cho bạn một jwt , khi đó bạn có thể dùng nó và thêm vào trong extras

> Các thông tin được tìm thấy ở dashboard 168chat.com/.
