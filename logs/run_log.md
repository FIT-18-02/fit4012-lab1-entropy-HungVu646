# Run Log – FIT4012 Lab 1

## Entropy / Redundancy
- [x] Đã chạy với input `aaaa`
- [x] Đã chạy với input `abcd`
- [x] Đã chạy với input `hello world`

## Modulo inverse
- [x] Đã chạy với `3 7`
- [x] Đã chạy với `10 17`
- [x] Đã chạy với `6 9`

## Điều em học được từ bài lab
Qua bài lab này, em đã hiểu rõ cách tính entropy của một chuỗi ký tự dựa trên tần suất xuất hiện, từ đó đánh giá được mức độ hỗn loạn và độ dư thừa thông tin – một khái niệm quan trọng trong lý thuyết thông tin. Em cũng thực hành thuật toán Euclid mở rộng để tìm nghịch đảo modulo, thấy được điều kiện cần và đủ là gcd(a, m) = 1. Khó khăn lớn nhất là lúc đầu chưa hình dung cách truy ngược các hệ số trong thuật toán đệ quy, nhưng việc chạy tay trên giấy với các bộ số cụ thể (như a=3, m=7) đã giúp em hiểu sâu hơn. Ngoài ra, xử lý phần dư âm để đưa kết quả về miền [0, m-1] cũng là một điểm cần chú ý. Nhìn chung, bài lab giúp em liên hệ giữa toán học rời rạc và ứng dụng thực tế trong mã hóa và an toàn thông tin
