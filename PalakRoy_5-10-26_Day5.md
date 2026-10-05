# BORZE
### SCREENSHOT
<img width="873" height="18" alt="image" src="https://github.com/user-attachments/assets/f11d9fea-eb00-4b21-902a-f8486aac7ce6" />

### CODE
```
#include <bits/stdc++.h>
using namespace std;

int main() {
    string s;
    cin >> s;

    for (int i = 0; i < s.size(); ) {
        if (s[i] == '.') {
            cout << '0';
            i++;
        } else {
            if (s[i + 1] == '.')
                cout << '1';
            else
                cout << '2';
            i += 2;
        }
    }

}
```
