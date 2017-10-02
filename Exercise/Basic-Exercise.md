
## Bài 1

Viết chương trình hiển thị ngày giờ theo format sau:
```
Today is: Friday
Current time is: 4 PM : 50 : 22
```

Note
- Sử dụng hàm getDay() để lấy số thứ tự về các ngày trong tuần (trả lại các giá trị từ 0-6 tương đương Sunday - Satturday)
- Sử dụng các hàm
  <ul>
  <li>getHours() lấy giờ</li>
  <li>getMinutes() lấy phút</li>
  <li>getSeconds() lấy giây</li>
  </ul>  




[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution01.html)

## Bài 2

Viết chương trình lấy ngày tháng sau đó định dạng lại với các định dạng sau:

```
mm-dd-yyyy
mm/dd/yyyy
dd-mm-yyyy
dd/mm/yyy
```

Note
- Sử dụng các hàm
  <ul>
  <li>getDate() to get Day = dd</li>
  <li>getMonth to get Month = mm , hàm này trả lại giá trị tháng (0-11) tương đương với (Jan - Dec)</li>
  <li>getFullYear()</li>
  </ul>
- Nếu số tháng hoặc số ngày < 10 thì thêm số 0 vào đằng trước giá trị `dd`, `mm`


[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution02.html)

## Bài 3

Viết chương trình tính diện tích tam giác với độ dài ba cạnh là 3,4,5:

Công thức Hê-rông [nguồn](https://vi.wikipedia.org/wiki/C%C3%B4ng_th%E1%BB%A9c_Heron)

<img src="https://image.prntscr.com/image/1Wo3nhKUSRuepKHWEy_D9Q.png">

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution03.html)

## Bài 4

Viết chương trình kiểm tra năm nhập vào có phải năm nhuận không?

Note:
- Năm nhuận là năm chia hết cho 4 
- Năm nhuận là năm chia hết cho 100 và chia hết cho 400

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution04.html)

## Bài 5

Tìm năm có chủ nhật là ngày đầu năm (ngày 01/01) trong khoảng từ năm 2014 đến năm 2050

Note:
- Một vòng lặp for từ năm 2014 đến năm 2050 với biến chạy `year`
- Khai báo một biến d - với ngày là ngày 1/1/year , `year` tương ứng với biến chạy của vòng lặp
- sử dụng hàm getDay(), nếu trả về giá trị bằng 0 thì là ngày chủ nhật
- In ra kết quả

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution05.html)

## Bài 6

Viết chương trình sinh ra một hàm random và người dùng sẽ đoán 1 số bất kỳ từ 1-10. Nếu đoán đúng sẽ hiển thị `Bingo`, nếu sai hiển thị `Failed`

Note
- Hàm *Math.ceil()* là hàm làm tròn
- Hàm *Math.random()* là hàm sinh ra một số ngẫu nhiên từ 0-1

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution06.html)

## Bài 7 

Viết chương trình tính số ngày còn lại đến ngày Giáng sinh

Note
- Ngày giáng sinh là ngày 25/11
- Hàm getTime() trả về milliseconds tính từ năm 01/01/1970
- Nếu ngày hôm nay là ngày 25/11 thì trả về giá trị 'Hôm nay là ngày giáng sinh'
- Nếu ngày hôm nay > ngày 25/11 thì biến FullYear thay đổi = +1, tức là giáng sinh gần nhất sẽ thuộc năm sau
- Một ngày = 1000*60*60*24 milliseconds
- Cách tốt nhất để tìm ngày còn lại là lấy ngày Giáng sinh đổi ra milliseconds trừ đi ngày hiện tại đổi ra miliseconds sau đó chia kết quả cho miliseconds của một ngày và làm tròn giá trị này. 

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution07.html)


## Bài 8 

Viết chương trình tính tích và thương 2 số nhập vào 2 ô textbox. Khi nhấn vào Multiply thì thực hiện phép nhân. Khi nhấn vào Divide thì thực hiện phép chia

<img src="https://image.prntscr.com/image/eb6y0EajQW_LdDgErWmHlA.png">

Note:
- document.getElementById('textBox1').value --> DOM lấy giá trị của document có id là `textBox1`
- !document.getElementById('textBox1').value --> check null
- document.getElementById("result").innerHTML --> insert dữ liệu vào document có id là `result`

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution08)

## Bài 9

Viết chương trình chuyển đổi qua lại giữa độ C và độ F

Note:
- Muốn đổi từ độ C sang độ F thì nhân với 1.8 rồi cộng thêm 32.
- Muốn đổi độ F sang độ C thì trừ đi 32, rồi chia cho 1.8

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution09.html)

## Bài 10

Viết chương trình lấy url của trang web:

Note
- Hàm document.URL --> dùng để lấy URL của trang hiện tại

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution10.html)

## Bài 11

Viết chương trình lấy tên phần mở rộng của file

` Ví dụ Explorer.exe ` --> trả về kết quả `exe`

Note 
- Method `split()` trả về kết quả là một mảng các phần tử phân cách nhau ở ví dụ này là dấu chấm (.). Nên có thể viết là 

```
var fileName = "Explorer.exe";
console.log(fileName.split('.'));
```

Kết quả trả về sẽ là `[Explorer, exe]`

- Method `pop()` trả về phần tử cuối cùng của một mảng

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution11.html)

## Bài 12

Viết chương trình so sánh một số với số 10. Nếu nhỏ hơn 10 thì in ra số đó. Nếu lớn hơn 10 thì in ra 2 lần hiệu của số lớn hơn - 10

Ví dụ số nhập vào là `20` kết quả sẽ là `(20-10)x2 = 20` 

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution12.html)

## Bài 13

Viết chương trình tính tổng hai số nguyên. Nếu hai số bằng nhau thì kết quả trả về là 3 lần tổng hai số

Note:
- Hàm validate có phải số không? có thể tham khảo tại [StackOverFlow](
https://stackoverflow.com/questions/469357/html-text-input-allows-only-numeric-input) hoặc [KeyCode-list](https://www.cambiaresearch.com/articles/15/javascript-char-codes-key-codes)

```
function validateNumber(evt) {
if (event.keyCode >= 48 && event.keyCode <= 57) {
    return true;
    } 
else 
     alert('Chỉ được nhập số, nếu cố tình nhập dấu chấm sẽ không nhận giá trị sau dấu chấm');
    }
```
- Sự kiện `onkeypress="return validateNumber(event)` sử dụng để bắt sự kiện khi bấm một phím nào đó trên bàn phím [Tham khảo](https://www.w3schools.com/jsref/event_onkeypress.asp)

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution13.html)

## Bài 14

Viết chương trình nhập vào một số và so sánh nó với số 19. Nếu lớn hơn thì trả về 3 lần hiệu của 2 số

Note

- Function `isNaN()` kiểm tra một giá trị có phải số không? Ví dụ `isNaN(19) = false`, `isNaN('huytm') = true`

[Tham khảo](https://www.w3schools.com/jsref/jsref_isnan.asp)

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution14.html)

## Bài 15

Viết chương trình kiểm tra số. Nếu một trong hai số bằng 50 hoặc tổng hai số bằng 50 thì trả kết quả về `true` !

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution15.html)

## Bài 16 

Viết chương trình kiểm tra hai số nhập vào. Nếu một số là âm và một số là dương thì trả kết quả là `true` !

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution16.html)

## Bài 17

Viết chương trình thêm chữ "Py" vào một chuỗi nhập vào. Nếu chuỗi đó bắt đầu bằng "Py" thì giữ nguyên chuỗi.

Note
- Hàm `substring(0,6)` để tìm 7 giá trị đầu tiên của chuỗi

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution17.html)

## Bài 18

Viết chương trình nhập vào một chuỗi sau đó xóa một ký tự bất kỳ ở chuỗi đó và trả về một chuỗi mới

Note
- Sử dụng hàm `substr()` chia thành hai chuỗi sau đó cộng hai chuỗi lại với nhau  

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution18.html)

## Bài 19

Viết chương trình đổi vị trí đầu tiên và cuối cùng của một chuỗi có từ 2 ký tự trở lên

Note 
- Tương tự ý tưởng như bài 18
- Phương thức String `charAt(0)` lấy giá trị của ký tự đầu tiên

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution19.html)

<a name="bai20"></a>
## Bài 20

Viết chương trình tạo ra một chuỗi mới bằng cách thêm ký tự đầu tiên của chuỗi cũ vào cả đầu và cuối chuỗi mới

Note
- Ý tưởng tương tự bài 19

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution20.html)

## Bài 21 

Viết chương trình kiểm tra một số có là bội của 3 và 7 không

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution21.html)

## Bài 22

Viết chương trình viết lại một chuỗi nhập vào bằng cách thêm vào trước và sau 3 ký tự cuối cùng của chuỗi ban đầu

- Note
Tương tự bài [20](#bai20)

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution22.html)

## Bài 23

Viết chương trình kiểm tra xem chuỗi nhập vào có bắt đầu bằng 'Java' không? Nếu có trả về `true`, nếu không trả về `false`. 

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution23.html)

## Bài 24 

Viết chương trình kiểm tra hai số có trong khoảng từ 50-99 không? Nếu một trong hai số thuộc thì trả về `true`, nếu không trả về `false`. 

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution24.html)

## Bài 25

Viết chương trình kiểm tra ba số xem có nằm trong khoảng từ 50 - 99 không? Nếu một hoặc nhiều hơn trong ba số thuộc thì trả về `true`, nếu không trả về `false`.

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution25.html) 

## Bài 26

Viết chương trình kiểm tra xem chuỗi nhập viết liền vào có chuỗi 'Script' (bắt đầu từ vị trí thứ 5 - index 4) hay không?. Nếu có 'Script' nằm ở vị trí như trên thì trả lại chuỗi không có chuỗi 'Script'. Nếu không thỏa mãn điều kiện trên thì giữa nguyên chuỗi.

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution26.html) 

## Bài 27

Viết chương trình tìm số lớn nhất trong 3 số nguyên

Note
- Hàm `Math.max()` tìm giá trị lớn nhất 

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution27.html) 

## Bài 28

Viết chương trình để tìm số có giá trị gần với 100 nhất từ hai số nhập vào

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution28.html) 

## Bài 29

Viết chương trình kiểm tra xem hai số có nằm trong khoảng từ 40-60 hoặc từ 70-100 không. Nếu có trả về `true`, nếu không trả về `false`

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution29.html) 

## Bài 30

Viết chương trình tìm số lớn nhất trong hai số nguyên dương nhập vào trong khoảng từ 40-70

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution30.html) 

## Bài 31

Viết chương trình tìm ký tự thứ 2 đến thứ 4 của một chuỗi có là kí tự mình cần tìm không. Ví dụ chuỗi `Python` hoặc `HuyTm` và ký tự cần tìm là `y` thì là `true`

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution31.html) 


## Bài 32 

Viết chương trình kiểm tra xem số hàng đơn vị của ba số nguyên nhập vào có giống nhau hay không?

Note
- Ba số có hàng đơn vị giống nhau đều chia cho 10 và dư giống nhau

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution32.html) 

## Bài 33 

Viết chương trình convert 3 ký tự đầu của một chuỗi là `low case` nếu chuỗi nhỏ hơn 3 ký tự thì chuyển cả chuỗi thành `up case`

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution33.html) 

## Bài 34

Viết chương trình phân loại học sinh với điểm trung bình. Nếu < 5 thì là "Yếu", 5-7 "Trung bình", 7-8 "Khá", 9-10 "Giỏi"

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution34.html) 

## Bài 35

Viết chương trình tính tổng hai số nguyên dương nếu kết quả nằm trong khoảng 60-80 thì trả về "65", nếu không trả về "80"

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution35.html) 

## Bài 36

Viết chương trình kiểm tra hai số, trả về `true` nếu một trong hai số bằng 8 hoặc hiệu hai số bằng 8.

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution36.html) 

## Bài 37 

Viết chương trình kiểm tra 3 số nhập vào. Nếu 3 số giống nhau thì trả về `30`. Nếu 2 số giống nhau thì trả về `20`. Nếu không thì trả về `40`

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution37.html) 

## Bài 38

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution38.html) 

Viết chương trình kiểm tra 3 số nhập vào có hàng đơn vị giống nhau không? Trả về `true` nếu 2 hoặc 3 số đều hàng đơn vị giống nhau. Trả về `false` nếu không có số nào có hàng đơn vị giống nhau

## Bài 39

Viết chương trình kiểm tra 2 số nguyên dương nhập vào. Trả về `true` nếu có tổng hoặc hiệu hai số bằng `15`

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution39.html) 

## Bài 40

Viết chương trình kiểm tra 2 số nhập vào. Trả về số bất kỳ trong hai số nếu số đó là bội của 11 hoặc 7

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution40.html) 

## Bài 41 

Viết đảo ngược chuỗi nhập vào

Note

- Method `split("")` --> nhét chuỗi vừa nhập vào một mảng với mỗi giá trị phân tách nhau bởi `("")`
- Method `reverse()` --> đảo ngược mảng 
- Method `join("")` --> nối các phần tử của mảng thành một chuỗi mà mỗi giá trị phân tách nhau bởi `("")`

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution41.html) 

## Bài 42 

Viết chương trình thay thế từng ký tự trong chuỗi cho trước bằng ký tự ngay sau nó trong bảng chữ cái

Note 

- Sử dụng [The ASCII Character Set](https://www.w3schools.com/charsets/ref_html_ascii.asp)
- Dùng hàm `String.fromCharCode(x)` để lấy ký tự thứ x theo bảng mã trên. Ví dụ `String.fromCharCode(65);` = `A`.
- Dùng hàm `charCodeAt(0)` để lấy số thứ tự trong bảng mã với ký tự đầu tiên của chuỗi. Ví dụ `"HelloWorld".charCodeAt(0);` kết quả = `72` tương ứng với chữ `H`, hoặc `"H".charCodeAt(0)` cũng bằng `72`.

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution42.html) 

## Bài 43 

Viết chương trình nhập vào một chuỗi sau đó viết hoa tất cả các chữ cái đầu tiên của một từ. Ví dụ `Have a nice day` = `Have A Nice Day`.

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution43.html) 

## Bài 44 

Viết chương trình nhập vào một chuỗi sau đó sắp xếp lại chuỗi đó theo bảng chữ cái

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution44.html) 

## Bài 45 

Viết một chương trình lặp lại chuỗi theo số lần mong muốn

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution45.html) 

## Bài 46 

Viết chương trình tạo ra chuỗi mới từ chuỗi nhập vào bằng cách x4 lần 3 kí tự cuối của chuỗi cũ. Chuỗi nhập vào phải > 3

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution46.html) 

## Bài 47

Viết chương trình lấy ra nửa đầu của một chuỗi nhập vào 

Note 
- Method `slice(a,b)` lây giá trị từ a - b trong chuỗi

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution47.html) 

## Bài 48

Viết chương trình nối hai chuỗi cho trước mà bỏ đi hai ký tự đầu tiên và cuối cùng của hai chuỗi.

Note 
- Hàm `substr(x,y)` lấy giá trị từ vị trí `x` đếm tiếp theo `y` ký tự. Ví dụ 

```
var str = "NguyenVietNam"
str.substr(1,5);
 
```

Kết quả là lấy từ vị trí thứ nhất - chữ `g` đếm tiếp (kể từ nó là 1) 5 ký tự --> kết quả là `guyen`

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution48.html) 

## Bài 49

Viết chương trình lấy ba ký tự giữa chuỗi (chuỗi phải là chuỗi có độ dài lẻ)

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution49.html)

## Bài 50

Viết chương trình kiểm tra chuỗi nhập vào trả lại tên thành phố, Ví dụ chuỗi nhập vào là `Ha` trả về `Ha Noi`

Note
- Ví dụ này trả về 3 thành phố là `HaNoi` `DaNang` `HoChiMinh`

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution50.html)
