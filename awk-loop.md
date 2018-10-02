:hotel: [Return to Home Page](https://github.com/geophydog/geophydog.github.io/blob/master/README.md)  
### 1. 一维循环
```awk
awk 'BEGIN{for(i=0;i<10;i++){print i}}'
```
#### output:
0  
1  
2  
3  
4  
5  
6  
7  
8  
9  

### 2. 二维（嵌套）循环
```awk
awk 'BEGIN{
        for(i=0;i<10;i++){
            for(j=0;j<10;j++){
                sum += i+j
            }
        }
        {print sum}
    }'
```
#### output:
900

### 3. 三维循环
```awk
awk 'BEGIN{
        for(i=0;i<10;i++){
            for(j=0;j<10;j++){
                for(k=0;k<10;k++){
                    sum += (i+j+k)
                }
            }
        }
        {print sum}
    }'
```
#### output:
13500

## 总结
-    __可见awk之for循环与c语言for循环类似，支持嵌套循环__
