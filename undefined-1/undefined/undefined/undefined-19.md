# 두 수의 연산값 비교하기

```swift
// Some code
import Foundation

func solution(_ a:Int, _ b:Int) -> Int {
    let xorResult = Int("\(a)\(b)")!
    let multiplicationResult = 2 * a * b
    
    if xorResult >= multiplicationResult {
        return xorResult
    } else {
        return multiplicationResult
    }
}
```
