# 문자열 정수의 합

```swift
import Foundation

func solution(_ num_str:String) -> Int {
    var sum = 0
    
    for char in num_str {
        if let digit = Int(String(char)) {
            sum += digit
        }
    }
    
    return sum
}
```
