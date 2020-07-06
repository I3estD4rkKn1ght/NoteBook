# for循环
## 死循环
```go
package main

import (
    "fmt"
    "time"
)

func main() {
    for {
        fmt.Println("进行循环")
        time.Sleep(time.Second * 1) // 延迟1s
    }
}
```
## 带条件的循环(布尔值 条件判断为布尔值)
```go
package main

import (
    "fmt"
    "time"
)

func main() { 
    for 2 > 1{  
        fmt.Println("进行循环")
        time.Sleep(time.Second * 1) // 延迟1s
    }
}
```
```go
package main

import (
    "fmt"
    "time"
)

func main() { 
    number := 1
    for number < 5 {  
        fmt.Println("进行循环")
        time.Sleep(time.Second * 1) // 延迟1s
        number += 1
    }
}
```

```go
package main

import (
    "fmt"
    "time"
)

func main() { 
    flag := true
    for flag {  
        fmt.Println("进行循环")
        time.Sleep(time.Second * 1) // 延迟1s
        flag = false
    }
}
```
