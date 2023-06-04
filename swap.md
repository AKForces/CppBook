交换两数的 ***5*** 中方法。
```cpp
#include <bits/stdc++.h>
using namespace std;
int a = 1, b = 2;
void swap1(int &a, int &b) // 利用函数。
{
    swap(a, b);
}
void swap2(int &a, int &b) // 借助第 3 个变量寄存。
{
    int temp = a;
    a = b;
    b = temp;
}
void swap3(int &a, int &b) // 求和，相减。
{
    a += b;
    b = a - b;
    a = a - b;
}
void swap4(int &a, int &b) // 求积，相除。
{
    a *= b;
    b = a / b;
    a = a / b;
}
void swap5(int &a, int &b) // 3 个异或。
{
    a = a ^ b;
    b = a ^ b;
    a = a ^ b;
}
void Print()
{
    cout << a << ' ' << b << '\n';
}
int main()
{
    Print();
    swap1(a, b); Print();
    swap2(a, b); Print();
    swap3(a, b); Print();
    swap4(a, b); Print();
    swap5(a, b); Print();
    return 0;
}
```
