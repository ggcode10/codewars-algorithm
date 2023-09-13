# 배열의 원소 삭제하기

```swift
import Foundation

func solution(_ arr:[Int], _ delete_list:[Int]) -> [Int] {
    
    var result:[Int] = []
    
    for num in arr {
        if !delete_list.contains(num) {
            result.append(num)
        }
    }
    return result
}
```
