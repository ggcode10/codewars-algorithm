# 자연수 뒤집어 배열로 만들기

```swift
func solution(_ n:Int64) -> [Int] {
    var str = String(n)
    var result: [Int] = []
    
    for i in str {
        result.append(Int(String(i))!)
    }
    result.reverse()
    return result
} 
```
