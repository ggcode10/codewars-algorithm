# 두 수의 합

## 풀이

for문으로 접근하면, 시간제한이 나오는 문제입니다. 투포인터로 해결하면 될 것 같습니다.

```swift
import Foundation

let N = Int(readLine()!)!
let arr = readLine()!.split(separator: " ").map{Int(String($0))!}.sorted()
let x = Int(readLine()!)!

var start = 0
var last = N - 1
var count = 0

while start < last {
    let target = arr[start] + arr[last]
    
    if target == x {
        count += 1
        start += 1
        last -= 1
    } else if target > x {
        last -= 1
    } else {
        start += 1
    }
}
print(count)

```
