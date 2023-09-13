# 콜라츠 추측

```swift
func solution(_ num:Int) -> Int {
    var count = 0
    var currentNum = num
    
    while currentNum != 1 {
        if count >= 500 {
            return -1
        }
        
        if currentNum % 2 == 0 {
            currentNum /= 2
        } else {
            currentNum = currentNum * 3 + 1
        }
        
        count += 1
    }
    
    return count
}
```
