# HTML-CSS-JS@Lab-04

#### Bài 1: Biến và hằng số
a. Khởi tạo biến a có gía trị bằng 10 và in ra màn hình console
b. Khởi tạo biến b có giá trị bằng ‘10’ và in ra màn hình console
c. Thay đổi giá trị của biến a thành 20 và in kết quả ra màn hình
d. Khởi tạo hằng số pi = 3.14 và in ra màn hình console
e. Thay đổi hằng số pi=5 và in ra màn hình console
f. Khởi tạo object điện thoại, với các thuộc tính sau: ten = iPhone 14, hangSanXuat = Apple, mauSac = Trang, gia = 1000USD và in ra màn hình console
g. Thay đổi giá của điện thoại từ 1000USD thành 750USD và in ra màn hình console
h. Thay đổi tên của điện thoại từ iPhone 14 thành iPhone 14 promax in ra màn hình console

#### Bài 2: Toán tử
a. Thực hiện phép tính tổng, hiệu, tích, thương của 2 nguyên a và b với a và b là 2 số nguyên được khởi tạo dưới dạng biến (giá trị tuỳ chọn)
b. Thực hiện phép tính trung bình cộng 2 số nguyên a và b, với a và b là 2 số nguyên được khởi tạo dưới dạng biến (giá trị tuỳ chọn)
c. Khởi tạo số nguyên x = 3, y = 4, z = 6 Tính giá trị các biểu thức sau:
- x^2 + 2x + 1
- x^3 – 3xy – 5y + 3y^2
- (xy)^2 – 2x^2*y + 13y
- 4x^3 + 3xy + y^2 – (2x^2 – 3y)
- (5x^2 / 4xy) + y^2
- x^2 – 2zxy / y^2 + 5x – 2y^2 + 4xz^3 + z^3

#### Bài 3: Cấu trúc rẽ nhánh `If-Else`
a. Viết hàm kiểm tra một số là số âm hay số dương.
b. Viết hàm kiểm tra một số là số chẵn hay số lẻ.
c. Viết hàm tìm số lớn nhất trong 3 số.
d. Viết hàm kiểm tra một năm có phải là năm nhuận hay không.
e. Viết hàm kiểu tra một kí tự là nguyên âm hay phụ âm
f. Viết hàm tìm nghiệm của phương trình bậc hai: `ax^2 + bx + c = 0` (Với a, b và c là 2 tham số được truyền vào hàm)
- Nếu a và b cùng bằng 0 thì phương trình vô nghiệm.
- Nếu a=0 thì phương trình có một nghiệm là (-c/b).
- Nếu b2-4ac < 0, thì phương trình vô nghiệm.
- Nếu không, phương trình có hai nghiệm, dùng công thức tính nghiệm để tính.
Lưu ý: Hàm tính căn bậc 2 trong js là: `Math.sqrt()`

g. Viết hàm tính thuế thu nhập và lương NET của nhân viên:
- 20% thuế thu nhập nếu lương từ 20 triệu trở lên
- 15% thuế thu nhập nếu lương trên 15 triệu đến 20 triệu
- 10% thuế thu nhập nếu lương từ 9 triệu đến 15 triệu
- 0% thuế thu nhập nếu lương dưới 9 triệu
Lưu ý: Tiền lương của nhân viên (Lương GROSS) sẽ được nhập vào từ tham số của hàm


#### Bài 4: Cấu trúc rẽ nhánh `Switch-Case`
a. Viết hàm nhập một số từ 1 tới 12 sau đó in ra màn hình tên tháng tương ứng.
     - Lưu ý: Nếu số nhập vào < 1 hoặc lớn hơn 12 thì phải thông báo lỗi
b. Viết hàm nhập vào số điểm theo thang điểm 100 và in ra xếp loại theo chữ cái với logic sau:
    - 90 – 100: Hạng A+
    - 80 – 89: Hạng A
    - 70 – 79: Hạng B
    - 60 – 69: Hạng C
    - Dưới 60: Hạng D
c. Viết hàm nhập 2 số và 1 phép toán (+, -, *, /) tính giá trị của của số với phép toán tương ứng.

d. Viết hàm nhập vào số từ 1 tới 12 sau đó in ra mùa tương ứng trong năm của tháng đó
- 3 -> 5: Mùa xuân
- 6 -> 8: Mùa hè
- 9 -> 11: Mùa thu
- 12 -> 2: Đông


e. Viết hàm nhập vào thể loại của bộ phim và tuổi của người xem, kiểm tra xem người đó có đủ tuổi để xem bộ phim đó không?
- Hành động (HD): trên 16 tuổi
- Kinh dị (KD): trên 18 tuổi
- Hài kịch (HK): Không giới hạn lứa tuổi
- Hoạt hình (HH): Không giới hạn lứa tuổi

#### Bài 5: Vòng lặp (for, while, do-while)
```js
let arr = [3, 451, 5, 2, 6, 76, 3, 5, 1, 243, 6, 4].
```
Hãy thực hiện các yêu cầu sau với mảng trên:
a. In ra màn hình console tất cả các phần tử của mảng
b. Tính tổng các phần tử trong mảng
c. Tìm phần tử lớn nhất, phần tử nhỏ nhất trong mảng
d. Tính trung bình cộng các phần tử trong mảng
f. Đảo ngược thứ tự các phần tử trong mảng
g. Tìm số lần xuất hiện của mỗi phần tử trong mảng
h. Chèn phần tử 117 vào đầu mảng
i. Kiểm tra xem mảng có phải là mỗi dãy số tăng dần hay không
k. Sắp xếp mảng theo thứ tự tăng dần
l. Sắp xếp mảng theo thứ tự giảm dần
m. Liệt kê danh sách các số chẵn trong mảng trên
n. Liệt kê danh sách các số lẽ trong mảng trên
