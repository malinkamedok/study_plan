# Павел Соловьев - задачи на собеседовании Biocad

1. Что будет выведено на экран?
   
```go
package main

import "fmt"

func main(){
    a := []int{1, 2, 3, 4, 5}
    a[1] = 4
    modify(a)
    fmt.Println(a)
}

func modify(a []int) {
    a[0] = 5
    a[3] = 2
    a = append(a, 0)
    a[4] = 1
}
```

2. Что будет выведено на экран?

```go
package main

import(
    "fmt"
    "time"
)

func main(){
    for i := 0; i < 10; i++ {
        go func(){
            fmt.Println(i)
        }()
    }
}
```

3. Написать функцию, которая преобразует строку в другой формат "aaaccbggggttttt" в "3a2c1b4g5t".