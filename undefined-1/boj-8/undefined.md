---
description: 백준 9012 괄호 문제와 동일합니다.
---

# 프로그래머스 - 올바른 괄호

```swift
// Some code
import Foundation

// count 변수 생성,  (일때 +1  ) 일때 -1
// count == 0이면 올바른 괄호 근데 () () ((일 경우도 생각
// count가 -인 경우는 바로 종료

var count = 0

func solution(_ s:String) -> Bool
{
    for target in s {
        if target == "(" {
            count += 1
        } else if target == ")" {
            count -= 1
            
            if count < 0 {
                break
            }
        }
    }
    
    if count == 0 {
        return true
    } else {
        return false
    }
}
```
