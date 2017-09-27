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

[Solution](https://github.com/huytm/Javascript/blob/master/Solution/solution11)
