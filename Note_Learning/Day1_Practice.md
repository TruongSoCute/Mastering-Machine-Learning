#### Thư viện Python
- ***Numpy***: đây là một thư viện viết bằng c và tối ưu nhanh hơn python.
	+ Thường được dùng để tính toán nhanh trên mảng, hoặc xử lý các dữ liệu số, cung cấp cho người dùng một cách tạo mảng nhanh chóng và thao tác trên nó ngắn gọn.
```python
	import numpy as np
	# tạo mảng array
	arr = np.array([1,2,3,4]);
	# thao tác với mảng nhanh
	print(arr * 2) # [2, 4, 6, 8]
	print(np.mean(arr)) #2.5
	# -------------------------- #
	# Tạo mảng với 10 phần tử ngẫu nhiên
	x = np.random.rand(10); 
	print(x)
	# [0.71698676 0.72160425 0.10765    0.54415177 0.93514684 0.12584851
	#  0.9264058  0.43120001 0.49964789 0.06974882]
```
+ ***Matplotlib:*** đây là thư viện thường được dùng để hiển thị sơ đồ như dạng *Scatter Plot, Pie Chart*
	+ .***pyplot***: Đây là module con của **Mathplotlib** là một module giúp người dùng dễ để vẽ ra các sơ đồ đơn giản hơn thay vì phức tạp như của thư viện cha.
	
```Python
import matplotlib.pyplot as plt
x = np.random.rand(50)
y = np.random.rand(50)
color = np.random.rand(50)
area = np.pi * (15 * np.random.rand(50)) ** 2 # S = Pi * R^2 
# 15 Được dùng để scale chỉ số cho bán kính hình tròn
plt.scatter(x,y, s=area, c=color, alpha=0.5) # In ra sơ đồ Scatter Plot có Diện tích hình tròn là S, chỉ số Color là C, Alpha là độ hiển thị = 0.5
# ở trên Parameter của chúng đề là mảng có length = 50 ta sẽ có kết quả ứng với giá trị của mỗi vị trí tương ứng các biến.
plt.show() # Hiển thị hình tròn
```
![Data](images/ScatterPlot_Day1.png)

+ ***IPython***: 
	+ **Display:** Dùng để hiển thị đẹp hơn với các dạng Array, HTML