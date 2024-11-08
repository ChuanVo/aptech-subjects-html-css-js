
# Cheatsheet HTML5

## 1. Cấu trúc cơ bản của tài liệu HTML5

HTML5 có cấu trúc cơ bản giúp trình duyệt hiểu được nội dung và hiển thị chính xác trên trang web. Dưới đây là một ví dụ về cấu trúc cơ bản:

```html
<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tiêu đề trang</title>
</head>
<body>
    <!-- Nội dung của trang sẽ được đặt ở đây -->
</body>
</html>
```

### Giải thích:
- `<!DOCTYPE html>`: Khai báo rằng tài liệu sử dụng HTML5. Đây là yêu cầu bắt buộc ở đầu mỗi trang HTML5.
- `<html lang="vi">`: Mở thẻ `<html>` và khai báo ngôn ngữ của trang là tiếng Việt (`vi`). Thẻ này là thẻ chứa toàn bộ nội dung HTML.
- `<head>`: Chứa thông tin mô tả trang web các thông tin này không hiển thị trực tiếp trên trang web.
- `<meta charset="UTF-8">`: Định dạng mã hóa ký tự UTF-8 giúp trang hiển thị chính xác các ký tự đa ngôn ngữ.
- `<meta name="viewport" content="width=device-width, initial-scale=1.0">`: Thiết lập chế độ xem cho thiết bị di động, điều chỉnh độ rộng của trang theo kích thước màn hình.
- `<title>`: Tiêu đề của trang, sẽ hiển thị trên tab trình duyệt.

---

## 2. Các Thẻ Nội Dung
> Dùng để trình bày nội dung chính trên trang

**2.1 Thẻ tiêu đề**
Thẻ `<h1>`, `<h2>`,... `<h6>`: Thẻ `<h1>` dành cho tiêu đề chính, và `<h2>` - `<h6>` cho các tiêu đề phụ.
```html
<h1>Tiêu đề chính</h1>
<h2>Tiêu đề phụ</h2>
```

**2.2 Đoạn văn**
Thẻ `<p>` dùng để viết đoạn văn bản.
```html
<p>Đây là một đoạn văn bản mẫu.</p>
```

**2.3 Danh sách**
  - **Danh sách có thứ tự**: Sử dụng thẻ `<ol>`, `<li>`
    ```html
    <ol>
        <li>Phần tử 1</li>
        <li>Phần tử 2</li>
    </ol>
    ```
  - **Danh sách không thứ tự**: Sử dụng thẻ `<ul>`, `<li>`
    ```html
    <ul>
        <li>Phần tử 1</li>
        <li>Phần tử 2</li>
    </ul>
    ```

**2.4 Bảng**
Thẻ `<table>` trong HTML được sử dụng để hiển thị dữ liệu dưới dạng bảng với các hàng và cột.

<b>Cấu trúc cơ bản:</b>
```html
<table>
    <caption>Tiêu đề của bảng</caption>
    <thead>
        <tr>
            <th>Cột 1</th>
            <th>Cột 2</th>
            <th>Cột 3</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Dữ liệu 1</td>
            <td>Dữ liệu 2</td>
            <td>Dữ liệu 3</td>
        </tr>
        <tr>
            <td>Dữ liệu 4</td>
            <td>Dữ liệu 5</td>
            <td>Dữ liệu 6</td>
        </tr>
    </tbody>
    <tfoot>
        <tr>
            <td colspan="3">Dữ liệu ở cuối bảng</td>
        </tr>
    </tfoot>
</table>
```

##### Giải thích:
  - `<table>`: Thẻ bao chứa toàn bộ bảng.
  - `<caption>`: Tiêu đề cho bảng, thường hiển thị phía trên bảng.
  - `<thead>`: Xác định phần đầu của bảng, chứa các hàng tiêu đề.
  - `<tbody>`: Chứa dữ liệu chính của bảng.
  - `<tfoot>`: Xác định phần cuối của bảng, thường để tổng hợp hoặc ghi chú.
  - `<tr>`: Đại diện cho một hàng trong bảng.
  - `<th>`: Tiêu đề của cột, thường in đậm và căn giữa theo mặc định.
  - `<td>`: Ô dữ liệu, chứa dữ liệu của bảng.

**2.5 Liên kết**
Thẻ `<a href="URL">` được sử dụng để tạo liên kết trong trang web.
```html
<a href="https://example.com">Trang web ví dụ</a>
```

**2.6 Hình ảnh**
Thẻ `<img src="URL" alt="Mô tả">` được sử dụng để thêm hình ảnh vào trang web.
```html
<img src="https://example.com/image.jpg" alt="Mô tả hình ảnh">
```

**2.7 Video**
Dùng thẻ `<video>` để nhúng video vào trang web.
```html
<video width="320" height="240" controls>
  <source src="movie.mp4" type="video/mp4">
</video>
```

**2.8 Audio**
Dùng `<audio>` để nhúng âm thanh vào trang web.
```html
<audio controls>
  <source src="horse.mp3" type="audio/mp3">
</audio>
```

**2.9 Canvas**
Dùng thẻ `<canvas id="myCanvas"></canvas>` dùng để vẽ đồ họa bằng JavaScript.

---

## 3. Thẻ Nhóm Nội Dung

Các thẻ này nhóm nội dung liên quan:
- **Div**: `<div>`: Nhóm nội dung thành các khối.
```html
<div class="myDiv">
  <h2>This is a heading in a div element</h2>
  <p>This is some text in a div element.</p>
</div>
```

- **Span**: `<span>`: Nhóm nội dung trong dòng.
```html
<p>My mother has <span style="color:blue">blue</span> eyes.</p>
```

- **Section**: `<section>`: Nhóm các phần nội dung có liên quan về ngữ nghĩa.
```html
<section>
  <h2>WWF History</h2>
  <p>The World Wide Fund for Nature (WWF) is an international organization working on issues regarding the conservation, research and restoration of the environment, formerly named the World Wildlife Fund. WWF was founded in 1961.</p>
</section>
```

- **Article**: `<article>`: Đoạn nội dung độc lập có thể tự tồn tại.
```html
<article>
  <h2>Mozilla Firefox</h2>
  <p>Mozilla Firefox is an open-source web browser developed by Mozilla. Firefox has been the second most popular web browser since January, 2018.</p>
</article>
```

- **Nav**: `<nav>`: Định nghĩa khu vực điều hướng.
```html
<nav>
  <a href="/html/">HTML</a>
  <a href="/css/">CSS</a>
  <a href="/js/">JavaScript</a>
  <a href="/python/">Python</a>
</nav>
```

---

## 4. Form và Các Thẻ Nhập Liệu

HTML cung cấp các thẻ để tạo biểu mẫu:
- **Form**: `<form action="URL" method="POST">`: Khởi tạo biểu mẫu.
```html
<form action="/action_page.php" method="POST">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Last name:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <input type="submit" value="Submit">
</form>
```

- **Input**: `<input type="text" name="tên" required>`: Thẻ `input` dùng để người dùng nhập liệu. Input có các kiểu như `text`, `email`, `password`.
```html
<input type="text" name="username" placeholder="Tên đăng nhập" required>
```

- **Select**: Tạo menu dropdown.
```html
<select name="options">
    <option value="1">Chọn 1</option>
    <option value="2">Chọn 2</option>
</select>
```

- **Button**: `<button>`: Hiển thị nút có thể nhấn được.
```html
<button type="button">Click Me!</button>
```

---

## 5. Thẻ Semantic

Các thẻ này giúp cải thiện SEO và khả năng truy cập:
- **Header**: `<header>`: Định nghĩa phần đầu trang.
```html
<article>
  <header>
    <h1>A heading here</h1>
    <p>Posted by John Doe</p>
    <p>Some additional information here</p>
  </header>
  <p>Lorem Ipsum dolor set amet....</p>
</article>
```

- **Footer**: `<footer>`: Định nghĩa phần cuối trang.
```html
<footer>
  <p>Author: Hege Refsnes</p>
  <p><a href="mailto:hege@example.com">hege@example.com</a></p>
</footer>
```

- **Aside**: `<aside>`: Nội dung phụ của trang.
```html
<p>My family and I visited The Epcot center this summer. The weather was nice, and Epcot was amazing! I had a great summer together with my family!</p>

<aside>
  <h4>Epcot Center</h4>
  <p>Epcot is a theme park at Walt Disney World Resort featuring exciting attractions, international pavilions, award-winning fireworks and seasonal special events.</p>
</aside>
```

- **Main**: `<main>`: Nội dung chính của trang.
```html
<main>
  <h1>Most Popular Browsers</h1>
  <p>Chrome, Firefox, and Edge are the most used browsers today.</p>

  <article>
    <h2>Google Chrome</h2>
    <p>Google Chrome is a web browser developed by Google, released in 2008. Chrome is the world's most popular web browser today!</p>
  </article>

  <article>
    <h2>Mozilla Firefox</h2>
    <p>Mozilla Firefox is an open-source web browser developed by Mozilla. Firefox has been the second most popular web browser since January, 2018.</p>
  </article>

  <article>
    <h2>Microsoft Edge</h2>
    <p>Microsoft Edge is a web browser developed by Microsoft, released in 2015. Microsoft Edge replaced Internet Explorer.</p>
  </article>
</main>
```

---

## 6. Thẻ Metadata

Các thẻ metadata cung cấp thông tin về trang web cho trình duyệt và công cụ tìm kiếm:

- **Meta Description**: `<meta name="description" content="Mô tả trang">`: Mô tả ngắn gọn về trang, giúp cải thiện SEO.
- **Meta Keywords**: `<meta name="keywords" content="HTML, CSS, JavaScript">`: Từ khóa của trang.
- **Meta Author**: `<meta name="author" content="Tên tác giả">`: Tên tác giả của trang.
