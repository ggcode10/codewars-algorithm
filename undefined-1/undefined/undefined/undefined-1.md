# 카운트 다운

```swift
import Foundation

func solution(_ start:Int, _ end:Int) -> [Int] {
    var my_list : [Int] = []

    for i in stride(from: start, to: end - 1, by: -1) {
        my_list.append(i)
    }
    return my_list
}
```
