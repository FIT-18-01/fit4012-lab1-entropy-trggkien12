# Report 1 Page – FIT4012 Lab 1

## 1. Mục tiêu
Thực hành và cài đặt thành công các thuật toán tính lượng tin (Entropy), độ dư thừa (Redundancy) và thuật toán Euclid mở rộng để tìm nghịch đảo modulo.

## 2. Cách làm
- Đọc hiểu chương trình entropy mẫu.
- Bổ sung hàm tính redundancy bằng công thức log2(N) - H(X).
- Hoàn thiện hàm mod_inverse() bằng thuật toán Euclid mở rộng và xử lý nghiệm dương.
- Chạy thử trên nhiều test case.

## 3. Kết quả chính
### 3.1 Entropy và redundancy
| Input | Entropy | Redundancy | Nhận xét |
|---|---:|---:|---|
| aaaa | 0 | 8 | Chuỗi có 1 ký tự duy nhất, độ bất định bằng 0, độ dư thừa cao nhất. |
| abcd | 2 | 6 | Các ký tự xuất hiện đều nhau, entropy tối đa cho chuỗi 4 ký tự. |
| hello world | ~3.16 | ~4.84 | Chuỗi phân bố ngẫu nhiên hơn nên độ dư thừa giảm đi. |

### 3.2 Modulo inverse
| a | m | Kết quả mong đợi | Kết quả chương trình |
|---:|---:|---|---|
| 3 | 7 | 5 | 5 |
| 10 | 17 | 12 | 12 |
| 6 | 9 | Không tồn tại | Không tồn tại |

## 4. Kết luận
Qua bài lab, em đã hiểu rõ hơn về cách đo lường lượng thông tin và nắm vững cách áp dụng thuật toán Euclid mở rộng trong toán học rời rạc/mật mã. Quá trình kiểm thử giúp củng cố kiến thức và tư duy xử lý lỗi.