# WORD CAPITALIZATION
### DESCRIPTION
Simple problem, just use toupper func

### SCREENSHOT
<img width="1781" height="27" alt="image" src="https://github.com/user-attachments/assets/355b3c06-8181-4a6b-bf19-3844c5256145" />

### CODE
```
#include <bits/stdc++.h>
using namespace std;


int main() {
    string s;
    cin >> s;

    s[0] = toupper(s[0]);
    cout << s;

}
```
