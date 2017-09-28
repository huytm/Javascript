
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




