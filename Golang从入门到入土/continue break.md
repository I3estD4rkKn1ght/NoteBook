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
for 循环 嵌套
```go
package main

import "fmt"

func main() {
	for i := 1; i < 10; i++ {
		for j := 1; j <= i; j++ {
			fmt.Printf("%d * %d = %d  ", j, i, i*j)
		}
		fmt.Println("")
	}
}
```
