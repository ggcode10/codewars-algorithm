# A 강조하기

문제를 꼼꼼히 읽지 않아 시간이 걸린 문제입니다.

```swift
import Foundation

func solution(_ myString:String) -> String {
    var result = ""

    for char in myString {
        if char == "a" || char == "A" {
            result += "A"
        } else if char.isUppercase {
            result += String(char.lowercased())
        } else {
            result += String(char)
        }
    }

    return result
}
```
