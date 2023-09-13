# 순서 바꾸기

```swift
import Foundation

func solution(_ num_list:[Int], _ n:Int) -> [Int] {
    var nList = num_list[n...]
    var mList = num_list[..<n]
    var result = Array(nList + mList)
    return result
}
```
