## 插入排序

### 描述

### 解析

### 实现代码

```javascript
let arr = [5,1,8,2,6,9,7,3,0,4];
for(let i = 1; i < arr.length; i++) {
    let temp = arr[i];
    let j = i;
    for(; j > 0; j--) {
      if(temp >= arr[j-1]) {
        break;      // 当前考察的数大于前一个数，证明有序，退出循环
      }
      arr[j] = arr[j-1]; // 将前一个数复制到后一个数上
    }
    arr[j] = temp;  // 找到考察的数应处于的位置
  }

//arr = [9, 8, 7, 6, 5, 4, 3, 2, 1, 0]
```

