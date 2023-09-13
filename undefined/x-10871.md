---
description: 백준 10871번
---

# X보다 작은 수 - 10871

## 문제

정수 N개의 수열 A에서 다음 인풋으로 주어지는 X보다 작은 수를 찾으면 된다.

## 접근

1. X는 처음 인풋의 1번 인덱스이다.
2. for 반복문은 input2를 순회한다.
3. X와 반복문 변수 i를 비교한다.
4. X보다 작은수를 Print한다.
5. `terminator` 를 사용하여 출력 형식에 맞게, 개행 제거하기

## 코드

```swift
import Foundation

// 정수 N개로 이루진 수열 A와 정수 X가 주어진다.
// A에서 X보다 작은 수를 모두 출력할 것

var input = readLine()!.split(separator: " ").map { Int($0)! }
var input2 = readLine()!.split(separator: " ").map { Int($0)! }
var X = input[1]

for i in input2 {
    if X > i {
        print(i, terminator: " ")
    }
}
```

