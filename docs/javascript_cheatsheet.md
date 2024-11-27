
# Tổng Quan Kiến Thức JavaScript

## 1. Giới Thiệu JavaScript
JavaScript là một ngôn ngữ lập trình được sử dụng rộng rãi trên cả phía **client** và **server**. Ban đầu, JavaScript được thiết kế để chạy trên trình duyệt web nhằm tạo hiệu ứng động và tương tác người dùng, nhưng với sự ra đời của **Node.js**, JavaScript đã trở thành một ngôn ngữ backend mạnh mẽ.

### Ứng dụng chính:
- Thao tác với DOM để cập nhật giao diện người dùng.
- Xử lý sự kiện (click, hover, form submit, v.v.).
- Gửi và nhận dữ liệu từ server thông qua AJAX hoặc Fetch API.
- Xây dựng ứng dụng web full-stack với Node.js.

---

## 2. Biến - Hằng số và Phạm vi của chúng
Sử dụng các từ khoá sau để khai báo:
- Biến: `var` hoặc `let`
- Hằng số: `const`

### Đặc điểm:
- `var`: 
  - Phạm vi **function-scoped** (giới hạn trong hàm chứa nó).
  - Có thể khai báo lại và bị **hoisting** (đưa lên đầu phạm vi).
- `let`: 
  - Phạm vi **block-scoped** (giới hạn trong cặp `{}`).
  - Không bị hoisting theo cách của `var`.
- `const`: 
  - Giống `let`, nhưng giá trị không thể thay đổi sau khi khai báo.

### Ví dụ:
```javascript
function testScope() {
    var x = 10; // Toàn hàm
    if (true) {
        let y = 20; // Block-scoped
        const z = 30; // Block-scoped, không thay đổi
        console.log(y, z); // Output: 20, 30
    }
    console.log(x); // Output: 10
}
testScope();
```

---

## 3. Kiểu Dữ Liệu
JavaScript có các kiểu dữ liệu cơ bản sau:

| **Loại Dữ Liệu** | **Ví Dụ**           | **Mô Tả**                                |
|-------------------|---------------------|------------------------------------------|
| `Number`          | `10`, `3.14`       | Số nguyên và số thực                     |
| `String`          | `"Hello"`          | Chuỗi ký tự                              |
| `Boolean`         | `true`, `false`    | Giá trị đúng hoặc sai                    |
| `Object`          | `{key: value}`     | Tập hợp các cặp key-value                |
| `Array`           | `[1, 2, 3]`        | Danh sách các giá trị                    |
| `Null`            | `null`             | Biến có giá trị null                   |
| `Undefined`       | `undefined`        | Biến chưa được gán giá trị               |

### Ví dụ:
```javascript
let num = 42;          // Number
let str = "Hello JS";  // String
let isTrue = true;     // Boolean
let person = { name: "John", age: 30 }; // Object
let numbers = [1, 2, 3]; // Array
let emptyValue = null;  // Null
let notAssigned;        // Undefined
```

---

## 4. Hàm (Functions)
Hàm là một khối mã thực thi một tác vụ cụ thể. Có hai cách khai báo hàm:

### 4.1 Hàm thông thường:
```javascript
function greet(name) {
    return \`Hello, \${name}!\`;
}
```

### 4.2 Hàm mũi tên (Arrow function):
Ngắn gọn hơn và không có `this` riêng.
```javascript
const greet = (name) => \`Hello, \${name}!\`;
```

**Ví dụ**:
```javascript
console.log(greet("Alice")); // Output: Hello, Alice!
```

---

## 5. Lập Trình Hướng Đối Tượng (OOP) Trong JavaScript
JavaScript hỗ trợ lập trình hướng đối tượng qua:
- **Class**: Cách dễ đọc để định nghĩa các đối tượng (introduced in ES6).
- **Prototype**: Mô hình kế thừa trước ES6.

### Ví dụ:
```javascript
class Vehicle {
    constructor(type, color) {
        this.type = type;
        this.color = color;
    }
    describe() {
        return \`This is a \${this.color} \${this.type}.\`;
    }
}

const car = new Vehicle("car", "red");
console.log(car.describe()); // Output: This is a red car.
```

---

## 6. Các Cấu Trúc Điều Khiển
### 6.1 Câu lệnh rẽ nhánh:
```javascript
let score = 85;

if (score >= 90) {
    console.log("Excellent");
} else if (score >= 70) {
    console.log("Good");
} else {
    console.log("Needs Improvement");
}
```

### 6.2 Vòng lặp:
#### Vòng lặp `for`:
```javascript
for (let i = 0; i < 5; i++) {
    console.log(i); // Output: 0 1 2 3 4
}
```

#### Vòng lặp `while`:
```javascript
let count = 0;
while (count < 3) {
    console.log(count++);
}
```

#### Vòng lặp `do-while`:
```javascript
let count = 0;
do {
    console.log(count++);
} while (count < 3)
```

---

# Thao Tác DOM Trong JavaScript

## 1. DOM Là Gì?
DOM (Document Object Model) là cấu trúc dữ liệu dạng cây, đại diện cho toàn bộ tài liệu HTML hoặc XML. JavaScript sử dụng DOM để truy cập và thay đổi cấu trúc hoặc nội dung của trang.

---

## 2. Truy Cập Các Phần Tử DOM
| **Phương Thức**                | **Mô Tả**                              |
|--------------------------------|----------------------------------------|
| `document.getElementById()`    | Lấy phần tử theo ID                    |
| `document.getElementsByClassName()` | Lấy danh sách phần tử theo class       |
| `document.querySelector()`     | Lấy phần tử đầu tiên khớp với selector |
| `document.querySelectorAll()`  | Lấy tất cả phần tử khớp với selector   |

**Ví dụ**:
```javascript
const button = document.querySelector("#myButton");
const items = document.querySelectorAll(".item");
```

---

## 3. Thay Đổi Nội Dung và Thuộc Tính
```javascript
const heading = document.querySelector("h1");
heading.textContent = "Updated Title"; // Thay đổi nội dung
heading.style.color = "blue";          // Thay đổi kiểu CSS
heading.setAttribute("class", "highlight"); // Thay đổi thuộc tính
```

---

## 4. Thêm và Xóa Phần Tử
**Thêm phần tử**:
```javascript
const newDiv = document.createElement("div");
newDiv.textContent = "New Content";
document.body.appendChild(newDiv);
```

**Xóa phần tử**:
```javascript
document.body.removeChild(newDiv);
```

---

## 5. Sự Kiện DOM
```javascript
button.addEventListener("click", () => {
    alert("Button clicked!");
});
```

---

## 6. Thao Tác Style
```javascript
const paragraph = document.querySelector("p");
paragraph.style.fontSize = "18px";
paragraph.style.backgroundColor = "yellow";
```

---

## Kết Luận
JavaScript là một ngôn ngữ đa năng và mạnh mẽ, không chỉ dành cho client mà còn có thể sử dụng trên server. Hiểu rõ JavaScript, đặc biệt là các thao tác với DOM, sẽ giúp bạn xây dựng được các ứng dụng web tương tác và hiện đại.
