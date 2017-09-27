Viết chương trình tính số ngày còn lại đến ngày Giáng sinh

Note
- Ngày giáng sinh là ngày 25/11
- Hàm getTime() trả về milliseconds tính từ năm 01/01/1970
- Nếu ngày hôm nay là ngày 25/11 thì trả về giá trị 'Hôm nay là ngày giáng sinh'
- Nếu ngày hôm nay > ngày 25/11 thì biến FullYear thay đổi = +1, tức là giáng sinh gần nhất sẽ thuộc năm sau
- Một ngày = 1000*60*60*24 milliseconds
- Cách tốt nhất để tìm ngày còn lại là lấy ngày Giáng sinh đổi ra milliseconds trừ đi ngày hiện tại đổi ra miliseconds sau đó chia kết quả cho miliseconds của một ngày và làm tròn giá trị này. 

[Solution](https://github.com/huytm/Javascript/new/master/Solution/solution7)
