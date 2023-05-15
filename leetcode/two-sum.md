# Two Sum

완전 탐색으로 접근하였습니다.

```swift
// Some code
class Solution {
    func twoSum(_ nums: [Int], _ target: Int) -> [Int] {
        // nums[i] + nums[j]가 target이라면
        for i in 0..<nums.count {
            for j in i+1..<nums.count {
                if nums[i] + nums[j] == target {
                    return [i, j]
                }
            }
        }
        return []
    }
}
```
