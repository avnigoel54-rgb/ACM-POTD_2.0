# Codeforces 492 A. **Vanya and Cubes**

## **Approach** - 
    -Calculate all three squared side lengths, sort them, and check the Pythagorean condition to detect a right triangle.
    -If not RIGHT, move each vertex one unit in the four possible directions and recheck.
    -Print ALMOST if any modification forms a right triangle; otherwise, print NEITHER.

## **Code** -
    
```cpp

#include <bits/stdc++.h>
using namespace std;

int main() {
    int n; cin >> n;
    int cnt = 0, curr = 0, i = 1;

    while (curr + i*i <= n) {
        cnt++;
        curr += i*i;
        i++;
    }

    cout << cnt;
}
```

![Output Screenshot](AvniGoel_03-11-26_Day34.png)
