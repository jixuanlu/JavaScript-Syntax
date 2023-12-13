# Map创建的方法
~~~
const map1 = new Map();   // 构造函数
~~~

# Map的常用方法
| return value | method | description |
| ------------ |--------|-------------|
| Map 对象 | set(key, value) | 向 Map 对象添加或更新一个指定的键值对 |
| undefined | clear() | 移除该 map 中的所有元素 |
| true/false | delete(key) | 从该 map 中删除指定键的元素 |
| 与指定键相关联的元素 | get(key) | 返回该 map 中的指定元素. 如果与所提供的键相关联的值是一个对象, 那么你将获得该对象的引用, 对该对象所做的任何更改都会有效地在 Map 对象中修改它 |
| true/false | has(key) | 返回一个布尔值, 指示具有指定键的元素是否存在 |

# Map传入参数为函数的方法
| return value | method | description |
| ------------ |--------|-------------|
| undefined | forEach(callbackFn) | 按插入顺序对该 map 中的每个键/值对执行一次提供的函数 callbackFn(value, key, map) |


# Map的迭代方法
| return value | method | description |
| ------------ |--------|-------------|
| 新的可迭代迭代器对象 | entries() | 返回一个新的 map 迭代器对象, 该对象包含了此 map 中的每个元素的 [key, value] 对, 按插入顺序排列 | 
| 新的可迭代迭代器对象 | keys() | 返回一个新的 map 迭代器对象, 该对象包含了此 map 中的每个元素的键, 按插入顺序排列 |
| 新的可迭代迭代器对象 | values() | 返回一个新的 map 迭代器对象, 该对象包含了此 map 中的每个元素的值, 按插入顺序排列 |
