### :one: 有分隔符情况  
_文件内容 test.txt_
```
AA a
BB b
CC c
DD d
EE e
FF f
```
_以" "为分隔符分割 _
```awk
awk '{split($0,arr," ");print arr[1], arr[2]}' test.txt
```
_output:_
```
AA a
BB b
CC c
DD d
EE e
FF f
```

### :two: 无分隔符
```awk
awk '{split($0,arr,"");print arr[1], arr[2], arr[4]}' test.txt
```
_output:_
```
A A a
B B b
C C c
D D d
E E e
F F f
```
