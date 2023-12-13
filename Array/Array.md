# 数组创建的方法
~~~
let arr = [];                           // 字面量
let arr = new Array("abc", 24, true);   // 构造函数
~~~

# 数组的常用方法
| method | description |
|--------|-------------|
| at(index) | 接收一个整数值并返回该索引对应的元素 |
| concat(arr0, arr1, … , arrN) | 用于合并两个或多个数组,此方法不会更改现有数组,而是返回一个新数组 |
| filter(callbackFn) | 返回满足筛选条件的新数组, callbackFn 是一个 function 它的传入值为 element(数组中当前正在处理的元素), index(正在处理的元素在数组中的索引), array(调用了 every() 的数组本身) |
| fill(value, start, end) | 用一个固定值填充一个数组中从起始索引（默认为 0）到终止索引(不包括)（默认为 array.length）内的全部元素,它返回修改后的数组 |
| find(callbackFn) | 返回数组中满足提供的测试函数的第一个元素的值, 否则返回 undefined |
| findIndex(callbackFn) | 返回数组中满足提供的测试函数的第一个元素的索引, 否则返回 -1 |
| findLast(callbackFn) | 反向迭代数组, 返回数组中满足提供的测试函数的第一个元素的值, 否则返回 undefined |
| findLastIndex(callbackFn) | 反向迭代数组, 返回数组中满足提供的测试函数的第一个元素的索引, 否则返回 -1 |
| every(callbackFn) | 测试一个数组内的所有元素是否都能通过指定函数的测试. 它返回一个布尔值, callbackFn 是一个 function 它的传入值为 element(数组中当前正在处理的元素), index(正在处理的元素在数组中的索引), array(调用了 every() 的数组本身) |
| copyWithin(target, start, end) | 浅复制数组的一部分到同一数组中的另一个位置,并返回它,不会改变原数组的长度, start 和 end 参数可选, 如果省略 start 则默认为 0, 如果省略 end 则默认为 array.length |
| flat(depth) | 创建一个新的数组，并根据指定深度递归地将所有子数组元素拼接到新的数组中, depth 可选, 默认为1 |
| map(callbackFn) | 创建一个新数组, 这个新数组由原数组中的每个元素都调用一次提供的函数后的返回值组成 |
| flatMap(callbackFn) | 对数组中的每个元素应用给定的回调函数, 然后将结果展开一级, 返回一个新数组. 它等价于在调用 map() 方法后再调用深度为 1 的 flat() 方法(arr.map(...args).flat()) |
| forEach() | 对数组的每个元素执行一次给定的函数, 返回值为 undefine | 
| includes() | 判断一个数组是否包含一个指定的值, 根据情况, 如果包含则返回 true, 否则返回 false | 
| indexOf(searchElement, fromIndex) | 返回数组中第一次出现给定元素的下标, 如果不存在则返回 -1, fromIndex 可选, 默认 0 |
| join() | 将一个数组（或一个类数组对象）的所有元素连接成一个字符串并返回这个字符串, 用逗号或指定的分隔符字符串分隔 |
| pop() | 从数组中删除最后一个元素, 并返回该元素的值. 此方法会更改数组的长度 |
| shift() | 从数组中删除第一个元素, 并返回该元素的值. 此方法更改数组的长度 |
| push() | 将指定的元素添加到数组的末尾, 并返回新的数组长度 |
| unshift() | 方法将指定元素添加到数组的开头，并返回数组的新长度 |
| reverse() | 就地反转数组中的元素, 并返回同一数组的引用 |
| slice(start, end) | 返回一个新的数组对象，这一对象是一个由 start 和 end 决定的原数组的浅拷贝(包括 start, 不包括 end), start 可选省略则为 0; end 可选省略则为arr.length|
| sort() | 默认排序是将元素转换为字符串, 然后按照它们的 UTF-16 码元值升序排序 | 
| toSorted(compareFn) | 对 number 进行排序: values.toSorted((a, b) => a - b) |

# 数组的迭代方法
| method | description |
|--------|-------------|
| entries() | 返回一个新的数组迭代器对象，该对象包含数组中每个索引的键(index)/值(value)对 |
| keys() | 返回一个新的数组迭代器对象，其中包含数组中每个索引的键 |
| values() | 返回一个新的数组迭代器对象, 该对象迭代数组中每个元素的值 |
~~~
const array1 = ['a', 'b', 'c'];
const iterator = array1.values();

for (const value of iterator) {
  console.log(value);
}
~~~

