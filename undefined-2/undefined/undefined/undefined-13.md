# 배열 비교하기

&#x20;문제에서 요구하는 사항에 맞추어 코드를 작성하면 됩니다.&#x20;

```swift
import Foundation

func solution(_ arr1:[Int], _ arr2:[Int]) -> Int {
    var arr1Sum = arr1.reduce(0, +)
    var arr2Sum = arr2.reduce(0, +)


    
    if arr1.count == arr2.count {
        if arr1Sum == arr2Sum {
            return(0)
        } else if arr1Sum > arr2Sum {
            return(1)
        } else {
            return(-1)
        }
    } else if arr1.count > arr2.count {
        return(1)
    }else {
        return(-1)
    }

}
```
