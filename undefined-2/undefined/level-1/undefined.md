# 약수의 합

```swift
// Some code
func solution(_ n:Int) -> Int {
    var arr: [Int] = []
    
    for i in 0...n {
        for j in 0...n {
            if i * j == n {
                arr.append(i)
            }
        }
    }
    return arr.reduce(0) { $0 + $1 }
}
```
