# Codeforces 44 A. **Indian Summer**

## **Approach** - 
    -Use set<string> to store only unique leaf descriptions (species + color).
    -Print st.size() to get the total number of unique leaves.

## **Code** -
    
```cpp

#include <bits/stdc++.h>
using namespace std;

  int main() {
      int n; cin >> n;
      string s;
      set<string> st;
      cin.ignore();
      for(int i=0;i<n;i++){
          s="";
          getline(cin,s);
          st.insert(s);
      }
      cout<<st.size();
  }

```

![Output Screenshot](AvniGoel_20-11-26_Day51.png)
