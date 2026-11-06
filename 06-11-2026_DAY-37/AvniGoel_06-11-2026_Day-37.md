# Codeforces 224 A. **Parallelepiped**

## **Approach** - 
    -Calculate the product a*b*c and find its square root t.
    -Use t/a, t/b, and t/c to determine the three edge lengths.
    -Apply the cuboid surface perimeter formula: 4 * (t/a + t/b + t/c).

## **Code** -
    
```cpp

#include <bits/stdc++.h>
using namespace std;

  int main() {
      long long a,b,c; cin>>a>>b>>c;
      long long prod = a*b*c;
      long long t=1;
      while(t*t<prod) t++;
      cout<< 4 * ((t/a)+(t/b)+(t/c));
  }


```

![Output Screenshot](AvniGoel_06-11-26_Day37.png)
