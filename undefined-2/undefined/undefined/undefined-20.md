# 콜라츠 수열 만들기

```swift
import Foundation

func solution(_ n:Int) -> [Int] {
    var result: [Int] = []
    var a = n
    result.append(a)
    
    while true {
        if a % 2 == 0 {
            a = a / 2
            result.append(a)
        } else if a % 2 == 1 {
            a = (3 * a) + 1
            result.append(a)
        }
        if a == 1 { break }
    }
    return result
}
```
