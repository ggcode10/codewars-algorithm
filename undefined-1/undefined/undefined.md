# 순서쌍의 개수

```swift
// Some code
func solution(_ n:Int) -> Int {
    return (1...n).filter{ n % $0 == 0 }.count
}
```
