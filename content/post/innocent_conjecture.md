+++
title = "A Conjecture on Linear Combinations of Rademacher Random Variables"

date = 2018-05-18
draft = false

tags = ["conjecture", "combinatorics", "probability theory"]
summary = "A seemingly innocent unsolved problem on the sum of Rademacher random variables (taking values $+ 1$ and $-1$ with equal probability $\\frac{1}{2}$)"

[header]
image = ""
caption = ""

+++
### 4.1. Bắt đầu với dữ liệu nhỏ
Các bài toán Machine Learning thường có độ phức tạp cao với lượng dữ liệu lớn và nhiều chiều. Để có thể áp dụng một thuật toán vào một bài toán cụ thể, trước tiên chúng ta cần áp dụng thuật toán đó vào _simulated data_ (dữ liệu giả) với số chiều và số điểm dữ liệu nhỏ hơn. _Simulated data_ này thường được tạo ngẫu nhiên (có thể thêm vài ràng buộc tùy vào đặc thù của dữ liệu). Với _simulated data_ nhỏ, chúng ta có thể debug nhanh hơn và thử với nhiều trường hợp _simulated data_ khác nhau. Khi nào thấy thuật toán chạy đúng chúng ta mới đưa _dữ liệu thật_ vào. 

Với Softmax Regression, tôi tạo _simulated data_ như sau: 

```python
import numpy as np 

# randomly generate data 
N = 2 # number of training sample 
d = 2 # data dimension 
C = 3 # number of classes 

X = np.random.randn(d, N)
y = np.random.randint(0, 3, (N,))
```
Trong ví dụ đơn giản này, số điểm dữ liệu chỉ là `N = 2`, số chiều dữ liệu `d = 2`, và số classes `C = 3`. Những giá trị đủ nhỏ này giúp cho việc kiểm tra có thể được thực hiện một cách tức thì. Sau khi thuật toán chạy đúng với những giá trị nhỏ này, ta có thể thay `N, d, C` bằng vài giá trị khác trước khi sử dụng dữ liệu thật. 

Dữ liệu \\(\mathbf{x}\\) có số chiều là \\((d +1)\\) vì có phần tử 1 được thêm vào phía trước, thể hiện hệ số tự do trong hàm tuyến tính. Hệ số tự do \\(w\_{0j}\\) còn được gọi là bias. 

Giả sử số classes là \\(C\\). Với one-vs-rest, chúng ta cần xây dựng \\(C\\) Logistic Regression khác nhau. Các _đầu ra dự đoán_ được tính theo hàm sigmoid:
\\[
a\_i = \text{sigmoid}(z\_i) = \text{sigmoid}(\mathbf{w}\_i^T\mathbf{x})
\\]
Trong kỹ thuật này, các phần tử \\(a\_i, i = 1, 2, \dots, C\\) được suy ra trực tiếp chỉ với \\(z\_i\\). Vì vậy, không có mối quan hệ chặt chẽ nào giữa các \\(a\_i\\), tức tổng của chúng có thể nhỏ hơn hoặc lớn hơn 1. Nếu ta có thể khai thác được mỗi quan hệ giữa các \\(z\_i\\) thì kết quả của bài toán classification có thể tốt hơn. 

Chú ý rằng các mô hình Linear Regression, PLA, Logistic Regression chỉ có 1 node ở output layer. Trong các trường hợp đó, tham số mô hình chỉ là 1 vector \\(\mathbf{w}\\). Trong trường hợp output layer có nhiều hơn 1 node, tham số mô hình sẽ là tập hợp 
tham số \\(\mathbf{w}\_i\\) ứng với từng node. Lúc này, ta có _ma trận trọng số_ \\(\mathbf{W} = [\mathbf{w}\_1, \mathbf{w}\_2, \dots, \mathbf{w}\_C]\\).