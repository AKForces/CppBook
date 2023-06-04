```cpp
#include <bits/stdc++.h>
using namespace std;
int main() {
    cout << (1 + 'a') << '\n';                      // int
    cout << ('a' + 1) << '\n';                      // int
    cout << ((1 == 0) + 'a') << '\n';               // int
    cout << ('a' + (1 == 0)) << '\n';               // int
    cout << ('a' + 3.0) << '\n';                    // double
    cout << (3.0 + 'a') << '\n';                    // double
    cout << (' ' + ' ') << '\n';                    // int
    cout << ((3 == 0) + 'a' + 1 + 3.0) << '\n';     // double
    cout << ((3 == 0) + (3 == 1)) << '\n';          // int
    cout << (false + false);                        // int
    return 0;
}
```
字符、布尔值参与了计算，都会被转化成 `int` 类型。
有小数参与运算，整个结构结果会转成 `double` 类型。
