# Codeforces 3 A. **Shortest path of the king**

## **Approach** - 
    -Calculate horizontal and vertical distance between the squares
    -Move diagonally using both directions for the minimum distance
    -Cover the remaining distance using the longer direction
    -Output total moves followed by each move in order

## **Code** -
    
```cpp
#include <bits/stdc++.h>
using namespace std;
  int main() {
  	char a1,b1,a2,b2;
  	cin>>a1>>b1>>a2>>b2;
  	int h_diff=a1-a2;
  	int v_diff=b1-b2;
  	char h=a1-a2<0?'R':'L';
  	char v=b1-b2<0?'U':'D';
  	int mn=min(abs(h_diff),abs(v_diff));
  	cout<<max(abs(h_diff),abs(v_diff))<<endl;
  	for(int i=0;i<mn;i++){
  	    cout<<h<<v<<endl;
  	}
  	char c;
  	if(abs(h_diff)>abs(v_diff))c=h;
  	else c=v;
  	int diff=max(abs(h_diff),abs(v_diff)) - min(abs(h_diff),abs(v_diff));
  	while(diff--){
  	    cout<<c<<endl;
  	}
  }

```

![Output Screenshot](AvniGoel_10-10-26_Day10.png)
