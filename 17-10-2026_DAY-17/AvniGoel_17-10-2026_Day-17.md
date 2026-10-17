# Codeforces 69 A. **Young Physicist**

## **Approach** - 
    -Initialize sums of x, y, and z to 0.
    -Add each force vector's components to their respective sums.
    -If all three sums are 0, print YES (equilibrium); otherwise, print NO.

## **Code** -
    
```cpp

#include <bits/stdc++.h>
using namespace std;

  int main() {
  
      int n; cin>>n;
      int a=0,b=0,c=0;
      while(n--){
          int x,y,z; 
          cin>>x>>y>>z;
          a+=x;
          b+=y;
          c+=z;
      }
      if(!a && !b && !c) cout<<"YES";
      else cout<<"NO";
  }

```

![Output Screenshot](AvniGoel_17-10-26_Day17.png)
