# Codeforces 492 A. **Vanya and Cubes**

## **Approach** - 
    -Each level requires i*(i+1)/2 cubes.
    -Keep adding complete levels while the remaining cubes are sufficient.
    -Increment cnt for each completed level and print the total height.

## **Code** -
    
```cpp

#include <bits/stdc++.h>
using namespace std;

int main() {
    int n;
    cin >> n;

    int cnt = 0, curr = 0, i = 1;

    while (curr + i*(i+1)/2 <= n) {
        cnt++;
        curr += i*(i+1)/2;
        i++;
    }

    cout << cnt;
}
```

![Output Screenshot](AvniGoel_03-11-26_Day34.png)
