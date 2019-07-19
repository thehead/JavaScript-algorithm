##选择排序

### 描述

### 解析

### 实现代码

```javascript
let arr = [5,1,8,2,6,9,7,3,0,4];
for(let i = 0;i < arr.length - 1;i++){
	let k = i; //记录最大或最小值的id，默认是循环第一个元素
  for(let j = i; j < arr.length; j++){
    if(arr[j]>arr[k]){  //从大到小排列取出最大值，反之条件取小与
      k = j;
    }
  }
  if(k != i){
		let temp = arr[i];
    arr[i] = arr[k];
    arr[k] = temp;
  }
}

//arr = [9, 8, 7, 6, 5, 4, 3, 2, 1, 0]
```

