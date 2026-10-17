# Is your horseshoe on the other hoof?
### DESCRIPTION
We use a set to remove the duplicate values and then subtract 4 and the size of set to get the answer.

### SCREENSHOT
<img width="875" height="21" alt="image" src="https://github.com/user-attachments/assets/313fcce3-32ae-466e-a84a-c345c749d7f5" />

### CODE
```
#include <bits/stdc++.h>
using namespace std;

int main() {
    int s[4];
    set<int> colors;

    for (int i = 0; i < 4; i++) {
        cin >> s[i];
        colors.insert(s[i]);
    }

    cout << 4 - colors.size() << endl;

}
```
