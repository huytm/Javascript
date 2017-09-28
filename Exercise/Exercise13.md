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

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution13)
