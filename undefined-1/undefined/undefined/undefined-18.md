# 간단한 식 계산하기

```swift
import Foundation

func solution(_ binomial:String) -> Int {
    var str = binomial.split(separator: " ")
    var A = Int(str[0])!, B = Int(str[2])!, op = str[1]
    if op == "+" {
        return A + B
    } else if op == "-" {
        return A - B
    } else if op == "*" {
        return A * B
    } else if op == "/" {
        return A / B
    } else {
        return A % B
    }
}
```
