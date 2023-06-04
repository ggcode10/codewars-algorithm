# n 번째 원소까지

swift에서 배열의 n번째 원소까지 출력하려면 arr\[..\<n] 이런식으로 슬라이싱 할 수 있습니다.

그러나 위의 방식은 아래 사진과 같이 \[Int] 형이 아닌, Array\<Int>.SubSequence형입니다.

문제에서 원하는 형식에 맞게 return 값을 \[Int] 형으로 맞춰주기 위해서는 위의 값을 담아줄&#x20;

새 정수형 배열이 필요합니다.

<figure><img src="../../.gitbook/assets/스크린샷 2023-06-04 오후 12.47.13.png" alt=""><figcaption><p>Array&#x3C;Int>.SubSequence</p></figcaption></figure>

## 코드&#x20;

```swift
import Foundation

func solution(_ num_list: [Int], _ n: Int) -> [Int] {

    var arr:[Int] = []
    arr.append(contentsOf: num_list[..<n])
    return arr
}
```
