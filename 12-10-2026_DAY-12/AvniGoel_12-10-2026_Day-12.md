# Codeforces 29 A. **Spit Problem**

## **Approach** - 
    -Store each point’s coordinates in a pair
    -Check every pair for mutual reflection conditions
    -Output YES if a valid pair exists, else NO

## **Code** -
    
```cpp
#include <bits/stdc++.h>
using namespace std;

  int main() {
  	int n; cin>>n;
  	vector<pair<int,int>> a(n);
  	int i=0,t=n;
  	while(t--){
  	    int x,d; cin>>a[i].first>>a[i].second;
  	    i++;
  	}
  	bool abc=false;
  	for(int i=0;i<n;i++){
  	    for(int j=i+1;j<n;j++){
  	        if(a[i].first==a[j].first+a[j].second && a[i].first+a[i].second==a[j].first){
  	            abc=true; break;
  	        }
  	    }
  	}
  	if(abc)cout<<"YES";
  	else cout<<"NO";
  }

```

![Output Screenshot](AvniGoel_12-10-26_Day12.png)
