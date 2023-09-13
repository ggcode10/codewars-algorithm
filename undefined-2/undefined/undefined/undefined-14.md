# 할 일 목록

```swift
import Foundation

func solution(_ todo_list:[String], _ finished:[Bool]) -> [String] {
    var nonTask:[String] = []
    
    for i in 0..<todo_list.count {
        if !finished[i] {
            nonTask.append(todo_list[i])
        }
    }
    return nonTask
}
```
