# SYSTEM OF EQUATIONS
### DESCRIPTION
We iterate through all possible values of a, calculate b = n - a^2 and count the no of pairs

### SCREENSHOT
<img width="875" height="18" alt="image" src="https://github.com/user-attachments/assets/de6ab24d-9fd9-45f1-b6c3-e1b15d87a286" />

### CODE
```

#include <bits/stdc++.h>
using namespace std;

int main() {
    int n, m;
    cin >> n >> m;
    int ct = 0;

    for (int a = 0; a*a <= n; a++){
        int b = n - (a*a);
        if (a+(b*b) == m) ct++;

    }
    cout << ct;
}
```
