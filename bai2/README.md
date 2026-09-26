1. Phân tích kĩ thuật

Dòng lệnh sai logic :
if (currentDrinkSize === "X") {
    break;
}

nếu dùng break -> những trường hợp bên dưới bị bỏ qua hết vì khi dùng break là dừng luôn 
Cách sửa : nên thay break = continue để đúng yêu cầu đầu bài

Các trường hợp testcase :
- Test case 1 : chuỗi có món hủy ở giữa
Input : giống đầu bài 
Output : 
Kết quả sai thực tế : Gặp X thì break , chỉ tính M + L
Kết quả đúng mong đợi : Bỏ qua X, tiếp tục tính M + L + S + M

- Test case 2 : chuỗi có món hủy ở cuối
Kết quả sai thực tế : Gặp X thì dừng vòng lặp 
Kết quả đúng mong đợi : Tính M + L + S bỏ qua X