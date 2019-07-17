## 冒泡排序

### 描述

### 解析

### 实现代码

~~~javascript
```
//目标数组
  let arr = [5,1,8,2,6,9,7,3,0,4];
	
  for(let i = 0; i < arr.length-1; i++){
    for(let j = 0; j < arr.length-1;j++){
      if(arr[j]>arr[j+1]){
        let temp = arr[j];
        arr[j] = arr[j+1];
        arr[j+1] = temp;
      }
    }
  }

```
~~~



### 优化

~~~javascript
```
  let arr = [5,1,8,2,6,9,7,3,0,4];
	
  for(let i = 0; i < arr.length-1; i++){
		let down = true;
    for(let j = 0; j < arr.length-1-i;j++){
      if(arr[j]>arr[j+1]){
        let temp = arr[j];
        arr[j] = arr[j+1];
        arr[j+1] = temp;
        down = false;
      }
    }
    if(down){
      break;
    }
  }

```
~~~







### 



