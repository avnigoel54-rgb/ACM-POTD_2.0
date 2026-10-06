# Codeforces 870 A. **Search for Pretty Integers**

## **Approach** - 
    -Store digits present in both sets using boolean arrays  
    -If a common digit exists, output the smallest one  
    -Otherwise, form the minimum two-digit number from the two minimum digits

## **Code** -
    
```cpp

#include <bits/stdc++.h>
using namespace std;
  int main() {
  	int n,m; cin>>n>>m;
  	int mn1=INT_MAX,mn2=INT_MAX;
  	vector<bool> a(10,false),b(10,false);
  	for(int i=0;i<n;i++){
  	    int x; cin>>x;
  	    mn1=min(mn1,x);
  	    a[x]=true;
  	}
  	for(int i=0;i<m;i++){
  	    int x; cin>>x;
  	    mn2=min(mn2,x);
  	    b[x]=true;
  	}
  	for(int i=0;i<10;i++){
  	    if(a[i] && b[i]){
  	        cout<<i;
  	        return 0;
  	    }
  	}
  	cout<<min(mn1,mn2)*10+max(mn1,mn2);
  }

```

![Output Screenshot](AvniGoel_07-10-26_Day7.png)
