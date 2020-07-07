# goto
跳跃到指定的行（位置），向下执行代码
```go
package main

import "fmt"

func main() {
	var name string
	fmt.Println("输入姓名")
	fmt.Scanln(&name)
	
	if name == "张三" {
		// svip 直接进
		goto SVIP
	} else if name == "李四" {
		// vip 
		goto VIP
	}
	fmt.Println("预约")
VIP:	
	fmt.Println("等号")
SVIP:	
	fmt.Println("进入")
}
```
定义位置 再goto跳到位置
