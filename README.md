# multiwork
A simple python multiprocessing tool

# Install

```
pip install multiwork
```

# Usage

### Source

``` python
import multiwork

datas = ["a","b","c","d","e"]

def pro(data, index):
	print data
	print index

# input data dictionary
# process count
# processing function
multiwork.run_multi(datas, 8, pro)
```

### Result
```
process 0 is start!
process 1 is start!
a
0
1 / 5
process 0 is end!
process 2 is start!
b
1
2 / 5
process 1 is end!
process 3 is start!
c
2
3 / 5
process 2 is end!
process 4 is start!
d
3
4 / 5
process 3 is end!
process 5 is start!
e
4
5 / 5
process 4 is end!
process 6 is start!
process 5 is end!
process 7 is start!
process 6 is end!
process 7 is end!
[Finished in 0.2s]
```

![process](https://github.com/subumm1/multiwork/blob/master/readme_process.png?raw=true)
