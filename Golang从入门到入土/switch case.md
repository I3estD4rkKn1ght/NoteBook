# switch case
帮助我们来做一些判断

表达式
```go
package main

import "fmt"

func main() {
    switch 表达式 {
    case 结果1:
        fmt.Println("结果1")
    case 结果2:
        fmt.Println("结果2")
    default:
        fmt.Println("都不满足")
    }
}
```
变量
```go
package main

import "fmt"

func main() {
    
    var age int
    fmt.Println("输入年龄:")
    fmt.Scanln(&age)
    switch age {
    case 15:
        fmt.Println("15")
    case 18:
        fmt.Println("18")
    default:
        fmt.Println("都不满足")
    }
}
```
