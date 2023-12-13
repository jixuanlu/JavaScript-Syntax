数组创建的方法
~~~
let arr = [];                           // 字面量
let arr = new Array("abc", 24, true);   // 构造函数
~~~

数组的常用方法
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
| entries() | 返回一个新的数组迭代器对象，该对象包含数组中每个索引的键(index)/值(value)对 |
