# Codeforces 36 A. **Extra-terrestrial Intelligence**

## **Approach** - 
    - Track the positions of consecutive 1s and calculate the distance between them.
    -Store the first distance and check if all subsequent distances are equal.
    -Print YES if all gaps match; otherwise, print NO.

## **Code** -
    
```cpp

#include <bits/stdc++.h>
using namespace std;

  int main() {
      freopen("input.txt", "r", stdin);
      freopen("output.txt", "w", stdout);
  
      int n;
      cin >> n;
  
      string s;
      cin >> s;
  
      int prev = -1, diff = -1;
  
      for(int i = 0; i < n; i++) {
          if(s[i] == '1') {
              if(prev != -1) {
                  if(diff == -1)
                      diff = i - prev;
                  else if(i - prev != diff) {
                      cout << "NO";
                      return 0;
                  }
              }
              prev = i;
          }
      }
  
      cout << "YES";
  }

```

![Output Screenshot](AvniGoel_23-11-26_Day54.png)
