# Report 1 Page – FIT4012 Lab 1

## 1. Mục tiêu
- Tính entropy của một chuỗi ký tự để đo mức độ hỗn loạn thông tin
- Tính độ dư thừa thông tin dựa trên entropy thực tế
- Cài đặt hàm tìm nghịch đảo modulo bằng thuật toán Euclid mở rộng

## 2. Cách làm
- Đọc hiểu chương trình entropy mẫu.
- Bổ sung hàm tính redundancy.
- Hoàn thiện hàm mod_inverse().
- Chạy thử trên nhiều test case.

## 3. Kết quả chính
### 3.1 Entropy và redundancy
| Input | Entropy | Redundancy | Nhận xét |
|---|---:|---:|---|
| aaaa | 0 | 8 | Chuỗi chỉ có một ký tự lặp lại → entropy = 0 , thông tin dư thừa tối đa |
| abcd | 2 | 6 | Bốn ký tự khác nhau, xác suất bằng nhau → entropy = log₂(4)=2, độ dư thừa giảm |
| hello world | 2.84535 | 5.15465 | Có ký tự lặp (l, o, space) làm entropy thấp hơn tối đa (8), redundancy còn cao |

### 3.2 Modulo inverse
| a | m | Kết quả mong đợi | Kết quả chương trình |
|---:|---:|---|---|
| 3 | 7 | 5 | 5 |
| 10 | 17 | 12 | 12 |
| 6 | 9 | Không tồn tại | "Không tồn tại nghịch đảo modulo vì gcd(a, m) != 1." (hoặc hàm trả về -1) |

## 4. Kết luận
Qua bài lab này, em đã hiểu được cách tính entropy của một chuỗi ký tự để đánh giá mức độ hỗn loạn của thông tin, từ đó xác định được độ dư thừa – một khái niệm quan trọng trong lý thuyết thông tin. Em cũng đã cài đặt thành công hàm tìm nghịch đảo modulo bằng thuật toán Euclid mở rộng, thấy rõ mối liên hệ giữa gcd(a,m) và sự tồn tại của nghịch đảo.Khó khăn lớn nhất là lúc đầu em chưa hình dung được cách truy ngược các hệ số x, y trong thuật toán Euclid mở rộng, dễ nhầm lẫn khi cập nhật giá trị. Tuy nhiên, chính việc chạy tay trên giấy với các bộ số cụ thể (ví dụ a=17, m=43) đã giúp em hiểu rõ cơ chế đệ quy và cách lấy phần dư âm về miền [0, m-1]. Đối với entropy, việc tính log2 của xác suất và so sánh kết quả với các chuỗi có độ dài khác nhau đã làm rõ tại sao chuỗi càng đều đặn thì entropy càng thấp và độ dư thừa càng cao


