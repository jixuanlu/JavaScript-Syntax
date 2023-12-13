# Set创建的方法
~~~
const set = new Set();   // 构造函数
~~~

# Set的常用方法
| return value | method | description |
| ------------ |--------|-------------|
| Set 对象 | add(value) | 在该集合中插入一个具有指定值的新元素 |
| undefined | clear() | 移除该集合中的所有元素 |
| true/false | delete(value) | 从该集合中删除指定值 |
| 与指定键相关联的元素 | get(key) | 返回该 Set 中的指定元素. 如果与所提供的键相关联的值是一个对象, 那么你将获得该对象的引用, 对该对象所做的任何更改都会有效地在 Set 对象中修改它 |
| true/false | has(value) | 返回一个布尔值来指示对应的值是否存在于该集合中 |

# Set的常用比较方法
| return value | method | description |
| ------------ |--------|-------------|
| Set 对象 | difference(other) | 返回一个新集合, 它包含了存在于当前集合但不存在于传入集合的元素 |
| Set 对象 | symmetricDifference() | 返回一个新集合, 它包含了存在于当前集合中且存在于传入集合中, 但不存在于两者交集中的元素 | 
| Set 对象 | intersection(other) | 接受一个集合返回当前集合与这个集合的交集组成的新集合 | 
| true/false | isDisjointFrom(other) | 返回一个布尔值来指示对应集合是否与当前集合有交集 | 
| true/false | isSubsetOf(other) | 返回一个布尔值来指示当前集合是否为传入集合的子集 |
| true/false | isSupersetOf(other) | 返回一个布尔值来指示传入集合是否为当前集合的子集 | 
| Set 对象 | union(other) | 返回一个新集合, 它包含了所有当前集合和传入集合元素 | 



# Set传入参数为函数的方法
| return value | method | description |
| ------------ |--------|-------------|
| undefined | forEach(callbackFn) | 按插入顺序为该集合中的每个值执行一次提供的函数 callbackFn(value, key, set) |


# Set的迭代方法
| return value | method | description |
| ------------ |--------|-------------|
| 新的可迭代迭代器对象 | entries() | 返回一个新的 Set 迭代器对象, 该对象包含了此 Set 中的每个元素的 [key, value] 对, 按插入顺序排列 | 
| 新的可迭代迭代器对象 | keys() | 返回一个新的 Set 迭代器对象, 该对象包含了此 Set 中的每个元素的键, 按插入顺序排列 |
| 新的可迭代迭代器对象 | values() | 返回一个新的 Set 迭代器对象, 该对象包含了此 Set 中的每个元素的值, 按插入顺序排列 |
