# 문자열 바꿔서 찾기

```swift
import Foundation

func solution(_ myString:String, _ pat:String) -> Int {
    var newStr = ""
    
    for str in myString {
        if str == "A" {
            newStr.append("B")
        } else if str == "B" {
            newStr.append("A")
        }
    }
    if newStr.contains(pat) {
        return 1
    } else {
        return 0
    }
}
```
