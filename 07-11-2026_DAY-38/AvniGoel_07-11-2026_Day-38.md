# Codeforces 270 A. **Fancy Fence**

## **Approach** - 
    -Calculate the required number of sides using the interior angle formula: 360 / (180 - a).
    -Check if 360 is divisible by (180 - a) to ensure the number of sides is an integer.
    -Print YES if divisible; otherwise, print NO.

## **Code** -
    
```cpp

#include <bits/stdc++.h>
using namespace std;

  int main() {
      int t; cin>>t;
      while(t--){
          int a; cin>>a;
          if(360%(180 - a)) cout<<"NO"<<endl;
          else cout<<"YES"<<endl;
      }
  
  }

```

![Output Screenshot](AvniGoel_07-11-26_Day38.png)
