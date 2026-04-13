# Test cases – FIT4012 Lab 1

Đánh dấu [x] khi đã chạy và kiểm tra kết quả.

## 1. Entropy / Redundancy
- [x] Input: `aaaa` -> entropy thấp, redundancy cao
- [x] Input: `aaaa` -> entropy thấp, redundancy cao
- [x] Input: `hello world` -> entropy và redundancy được tính hợp lệ

## 2. Modulo inverse
- [x] `a=3, m=7` -> nghịch đảo modulo là 5
- [x] `a=10, m=17` -> nghịch đảo modulo là 12
- [x] `a=6, m=9` -> không tồn tại nghịch đảo modulo     

## 3. Ghi chú   
- Entropy / Redundancy
Input: `i love you` -> entropy(2.92193) và redundancy(5.07807) được tính hợp lệ
Input: `abcdabcd` -> entropy(2) thấp, redundancy(6) cao
- Modulo inverse
`a=12, m=17` -> nghịch đảo modulo là 10
`a=32, m=77` -> nghịch đảo modulo là 65
`a=21, m=29` -> nghịch đảo modulo là 18
`a=33, m=77` -> không tồn tại nghịch đảo modulo
