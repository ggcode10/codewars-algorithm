# 이어 붙인 수

런타임 에러가 나올수도 있습니다.

```swift
import Foundation

func solution(_ num_list:[Int]) -> Int {
    var oddNum: [Int] = []
    var evenNum: [Int] = []
    
    for i in num_list {
        if i % 2 == 0 {
            evenNum.append(i)
        } else if i % 2 == 1 {
            oddNum.append(i)
        }
    }
    var sum1 = evenNum.map { String($0) }.joined(separator: "")
    var sum2 = oddNum.map { String($0) }.joined(separator: "")
    return (Int(sum1)! + Int(sum2)!)
}
```
