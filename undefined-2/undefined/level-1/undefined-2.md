# 하샤드 수

```swift
func solution(_ x:Int) -> Bool {
    var strX = String(x).compactMap{ Int(String($0)) }
    var reduce = strX.reduce(0, +)
    
    if x % reduce == 0 {
        return true
    } else {
        return false
    }
}
```
