# continue break
## continue
在for循环中使用，当循环遇到continue时，会跳过当前循环，开始下一次循环
```go
package main

import "fmt"

func main() {
    for {
        fmt.Println("aaa")
        continue
        fmt.Println("bbb")
    }
}
```
```go
package main

import "fmt"

func main() {
    for i := 1; i <= 10; i++ {
        if i == 7 {
            continue
        }
        fmt.Println(i)
    }
}
```
for 循环 嵌套 + continue
```go
package main

import "fmt"

func main() {
    for i := 1; i <= 10; i++ {
    	if i == 10 {
	    continue
	}
	for j := 1; j <= i; j++ {
	    fmt.Printf("%d * %d = %d  ", j, i, i*j)
	}
	fmt.Println("")
    }
}
```

## break
在for循环中一旦遇到break，跳出循环
```go
for i := 1; i < 10; i++{
    fmt.Println(i)
    if i == 5 {
    	break
    }
}
```
猜数字
```go
package main

import "fmt"

func main() {
    data := 66
    var userNum int
    for {
    	fmt.Print("输入一个数字:")
	fmt.Scanln(&userNum)
	if userNum == data {
	    fmt.Println("恭喜你，答对了")
	    break
	} else if userNum > data {
	    fmt.Println("很遗憾，答错了,比答案大了")
	} else {
	    fmt.Println("很遗憾，答错了,比答案小了")
	}
    }
}
```
