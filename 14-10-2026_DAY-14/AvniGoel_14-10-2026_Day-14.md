# Codeforces 312 B. **Archer**

## **Approach** - 
    -Calculate each player's probability of scoring on one attempt
    -Find the probability that both players fail in a round\
    -Use the geometric series to calculate the probability that the first player scores first
    -Output the result with precision of 10 decimal places

## **Code** -
    
```cpp
#include <bits/stdc++.h>
using namespace std;

  int main() {
  	double a,b,c,d; cin>>a>>b>>c>>d;
  	double p=a/b;
  	double q=c/d;
  	double r=(1-p)*(1-q);
  	double ans=p/(1-r);
  	cout<<fixed<<setprecision(10)<<ans;
  }

```

![Output Screenshot](AvniGoel_14-10-26_Day14.png)
