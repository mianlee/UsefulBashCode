# UsefulBashCode

Here is the repo that I use to record useful bash codes during my learning.

#
```
# 查看文件夹和文件大小
du -h 

# 一次建立多个文件夹

mkdir {apple, pear, peach}

# find

find /folder/ -name *.gz

# xargs, xargs 结合 find 使用

find /folder/ -name *gz | xargs ls -la


# mkdir -p

mkdir -p /folder/subfolder/ && cd /folder/subfolder/

```


```
#basename 函数， 引号中是要去掉的内容


(basename $id ".gz")


```


```
#($id) 是用来给指定文件分类的

cat config 
apple red round
pear blue square
peach green triangle


cat config | while read id

do
arr=($id)
fg1=${arr[0]}
fg2=${arr[1]}
fg3=${arr[2]} 
echo $fg1
done

#result
apple
pear
peach
```
