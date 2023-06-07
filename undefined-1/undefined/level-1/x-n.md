# x만큼 간격이 있는 n개의 숫자

```swift
func solution(_ x:Int, _ n:Int) -> [Int64] {
    var arr: [Int64] = []
    var count = 0
    
    while true {
        count += x
        arr.append(Int64(count))
        
        if arr.count == n { break }
    }
    return arr
}
```
