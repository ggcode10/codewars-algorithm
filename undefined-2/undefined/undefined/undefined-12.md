# 배열의 길이에 따라 다른 연산하기

```swift
import Foundation

func solution(_ arr:[Int], _ n:Int) -> [Int] {
    var newArr = arr
    for (index, num) in arr.enumerated() {
        if arr.count % 2 == 1 && index % 2 == 0 {
            newArr[index] = num + n
        } else if arr.count % 2 == 0 && index % 2 == 1 {
            newArr[index] = num + n
        }
    }
    return newArr
}
```
