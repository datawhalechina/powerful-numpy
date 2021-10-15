## CheatSheet

此处罗列部分相关 API 用法，以二维为主，多维可自行拓展。


| 说明 | 用法 |
|------|-----|
||**创建和生成**|
|从list创建|`np.array(list)`|
|从range创建|`np.arange(int).reshape(int, int, ...)`|
|按线性间隔创建|`np.linspace(start, stop, num).reshape(int, int)`|
|从对数间隔创建|`np.logspace(start, stop, num, base).reshape(int, int)`|
|全1|`np.ones(int)`|
|全0|`np.zeros((int, int, ...))`|
|和给定array同shape的0向量|`np.zeros_like(array)`|
|随机 Generator|`rng = np.random.default_rng()`|
|随机整数|`rng.integers(low, high, (int, int))`|
|均匀分布|`rng.uniform(low, high, (int, int))`|
|标准正态分布|`rng.standard_normal((int, int))`|
|高斯分布|`rng.normal(loc, scale, (int, int))`|
|存储单个array|`np.save(file, array)`|
|存储多个array|`np.savez(file, name=array)`|
|存储多个array并压缩|`np.savez_compressed(file, name=array)`|
|加载|`np.load(file)`|
||**统计和属性**|
|维度|`arr.ndim`|
|形状|`arr.shape`|
|尺寸|`arr.size`|
|按维度取最大值|`arr.max(aixs)`|
|按维度取最小值并保持维度|`arr.min(axis, keepdims=True)`|
|中位数|`np.median(arr)`|
|分位数|`np.quantile(arr, q, axis)`|
|求和|`np.sum(arr)`|
|按维度求均值|`np.average(arr, axis)`|
|按维度求累加和|`np.cumsum(arr, axis)`|
||**形状和转换**|
|改变形状|`arr.reshape(int, int, ...)`|
|原地改变|`arr.resize(int, int, ...)`|
|打平|`arr.ravel()`|
|扩展1维度|`np.expand_dims(arr, axis)`|
|去掉1维度|`np.squeeze(arr, axis)`|
|反序|`arr[::-1]`|
|列反序|`arr[:, ::-1]`|
|行反序|`arr[::-1, :]`|
|二维转置|`arr.T`|
|高维转置|`np.transpose(arr, axes)`|
||**分解和组合**|
|索引|`arr[int]`|
|范围索引|`arr[int: int]`|
|离散索引|`arr[[int, int]]`|
|范围+离散|`arr[int:int, int]`|
|范围+范围|`arr[int:int, int:int]`|
|离散+离散|`arr[[int, int], [int, int]]`|
|步长跳跃|`arr[start: end: step]`|
|多维度步长跳跃|`arr[start: end: step, start: end: step]`|
|按维度拼接|`np.concatenate((arr1, arr2), axis)`|
|按维度堆叠|`np.stack((arr1, arr2), axis)`|
|重复|`np.repeat(arr, int, axis)`|
|按维度切分|`np.split(arr, parts, axis)`|
||**筛选和过滤**|
|筛选|`np.where(condition)`|
|筛选后赋值|`np.where(condition, arr, not_satisfy_condition_with_new_val)`|
|提取|`np.extract(condition, arr)`|
|唯一值|`np.unique(arr)`|
|抽样|`np.random.choice(arr, int, bool)`|
|按维度取最大值index|`np.argmax(arr, axis)`|
|按维度排序的索引|`np.argsort(arr, axis)`|
||**矩阵和运算**|
|四则运算| `arr [+-*/] num`                 |
|其他运算 | `np.[sqrt/floor/round/mod](arr)` |
|array乘法| `np.dot(arr1, arr2)`             |
|array乘法| `np.matnul(arr1, arr2)`          |
|点积     | `np.vdot(arr1, arr2)`            |
|内积     | `np.inner(arr1, arr2)`           |
|行列式   | `np.linalg.det(arr)`             |
|逆矩阵   | `np.linalg.inv(arr)`             |

