# 접미사 배열

```swift
// Some code
func solution(_ my_string: String) -> [String] {
    var result:[String] = []
    
    for i in 0..<my_string.count {
        let mySuffix = String(my_string.suffix(from: my_string.index(my_string.startIndex, offsetBy: i)))
        result.append(mySuffix)
    }
    var sortedResult = result.sorted()
    return sortedResult
}
```
