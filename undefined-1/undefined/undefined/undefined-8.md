# 첫 번째로 나오는 음수

```swift
import Foundation

func solution(_ num_list:[Int]) -> Int {
    for (index, num) in num_list.enumerated() {
        if num < 0 {
            return index
        }
    }
    return -1
}
```
