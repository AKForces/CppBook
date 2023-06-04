`else` 是找前面最近的且能配套的 `if` 语句配套。
```cpp
#include <bits/stdc++.h>
using namespace std;
int main()
{
    int n;
    cin >> n;
    if (1 <= n && n <= 100)//<-------------------------------------
        if (n <= 50) // <--------------                           |
            cout << "n <= 50\n"; //   |                           |  
        else // 跟最近的 if 匹配。 ------                            |
            cout << "n >= 51"; //                                 |
    else cout << "overflow\n"; // 与最近的 && 可以匹配的匹配 ---------
}
```
