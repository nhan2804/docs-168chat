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
        fullname: "Name of user",
        age: 21,
        more: "more and more",
      },
    });
</script>
```

> Các thông tin được tìm thấy ở dashboard 168chat.com/.
