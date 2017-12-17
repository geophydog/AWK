```
Just included by '''${xxx}'''
```

```shell
for(i=0;i<=10;i++);do
  echo "A B C" | awk '{print $1,'''${i}'''}'
done
```
