# 글자 이어 붙여 문자열 만들기

```swift
// Some code
import Foundation

var my_string:String = "cvsgiorszzzmrpaqpe"
var index_list:[Int] = [16, 6, 5, 3, 12, 14, 11, 11, 17, 12, 7]
var result = ""

for index in index_list {
    if index >= 0 && index < my_string.count {
        let charStr = my_string.index(my_string.startIndex, offsetBy: index)
        let char = my_string[charStr]
        result.append(char)
    }
}

```
