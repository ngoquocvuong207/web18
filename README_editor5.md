# Editor 5: Báo cáo Network Tab

Bài tập tạo trang HTML chứa bảng ghi lại kết quả Network Tab của DevTools: tên tài nguyên, loại, ai gửi yêu cầu (initiator), ai trả phản hồi (server), trạng thái, dung lượng, thời gian tải.

---

## Yêu cầu bài tập

- Tạo bảng ghi tên tài nguyên, loại tài nguyên, ai gửi yêu cầu, ai trả phản hồi
- Dựa vào yêu cầu ghi chép kết quả thực hành Network tab (DevTools)
- Tự gõ, test trên editor online, đẩy GitHub Pages, nộp 2 link

---

## Cấu trúc file

```
project/
└── index.html
```

---

## Kiến thức cốt lõi: Network Tab

### Các cột quan trọng trong Network Tab

| Cột | Tên tiếng Anh | Ý nghĩa |
|-----|---------------|---------|
| Tên tài nguyên | Name | Tên file được tải (index.html, style.css...) |
| Loại | Type | Loại tài nguyên: document, stylesheet, script, image, font, fetch |
| Ai gửi yêu cầu | Initiator | Cái gì khởi tạo request (browser, thẻ HTML, JS...) |
| Ai trả phản hồi | Server / Remote Address | Server nào phản hồi (web server, CDN, API...) |
| Trạng thái | Status | HTTP status code (200, 304, 404...) |
| Dung lượng | Size | Kích thước file nhận về |
| Thời gian | Time | Tổng thời gian tải |

### Các loại tài nguyên (Type)

| Loại | Ví dụ | Initiator phổ biến |
|------|-------|--------------------|
| `document` | index.html | Browser (address bar, click link) |
| `stylesheet` | style.css | `<link rel="stylesheet">` trong HTML |
| `script` | main.js | `<script src="...">` trong HTML |
| `image` | logo.png | `<img src="...">` hoặc CSS background |
| `font` | Roboto.woff2 | `@font-face` hoặc Google Fonts |
| `fetch` / `xhr` | api/data.json | `fetch()` hoặc `XMLHttpRequest` trong JS |

### HTTP Status Code thường gặp

| Code | Nghĩa | Khi nào gặp |
|------|-------|-------------|
| 200 | OK — thành công | Tài nguyên tải bình thường |
| 301 | Moved Permanently | Chuyển hướng vĩnh viễn |
| 304 | Not Modified | Dùng cache, không tải lại |
| 404 | Not Found | File không tồn tại |

---

## Tính năng của file mẫu

| Tính năng | Mô tả |
|-----------|-------|
| Summary cards | Tổng số request, dung lượng, thời gian, tỉ lệ thành công |
| Bảng Network | 8 hàng mẫu gồm document, CSS, JS, image, font, fetch, 404 |
| Size bar | Thanh biểu đồ trực quan so sánh dung lượng |
| Nút lọc | Click để lọc theo loại tài nguyên |
| Màu badge | Mỗi loại có màu riêng dễ phân biệt |

---

## Cách nộp bài

1. Tạo repo mới trên GitHub
2. Upload `index.html`
3. **Settings → Pages → Branch: main → Save**
4. Nộp 2 link:
   - Repo: `https://github.com/username/repo-name`
   - Pages: `https://username.github.io/repo-name`

---

## Checklist trước khi nộp

- [ ] File tên là `index.html`
- [ ] Có bảng ghi tên tài nguyên, loại, initiator, server, status
- [ ] Có ít nhất 5 loại tài nguyên khác nhau
- [ ] Trang chạy đúng trên editor online
- [ ] GitHub Pages truy cập được
- [ ] Đã nộp đủ 2 link
