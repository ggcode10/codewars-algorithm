# 핸드폰 번호 가리기

```swift
func solution(_ phone_number:String) -> String {
    let count = phone_number.count
    var result = ""
    for (index, digit) in phone_number.enumerated() {
        if index < count - 4 {
            result.append("*")
        } else {
            result.append(digit)
        }
    }
    return result
}
```
