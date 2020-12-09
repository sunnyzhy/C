## 数据类型长度
|类型|32位平台(x86)|64位平台(x64)|
|--|--|--|
|char|1|1|
|short|2|2|
|int|4|4|
|long|4|4|
|long long|8|8|
|float|4|4|
|double|8|8|
|size_t|4|8|

## malloc

使用 malloc 从堆上申请内存之后，**如果修改了所分配内存以外的内存**，在调用 free() 的时候就会产生异常：**CRT detected that the application wrote to memory after end of heap buffer**
