# 마지막 두 원소

```swift
import Foundation

func solution(_ num_list:[Int]) -> [Int] {
var result = num_list
    
    if num_list.count >= 2 {
        let lastElement = num_list.last!
        let prevElement = num_list[num_list.count - 2]
        
        if lastElement > prevElement {
            let subtractedValue = lastElement - prevElement
            result.append(subtractedValue)
        } else {
            let doubledValue = lastElement * 2
            result.append(doubledValue)
        }
    }
    
    return result
}

```
