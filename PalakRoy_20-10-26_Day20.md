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
# STRING TASK
### DESCRIPTION
We check if the letter isn't a vowel and then output it with the . and the letter. We also first convert all letters to lowercase. 

### SCREENSHOT
<img width="1758" height="37" alt="image" src="https://github.com/user-attachments/assets/e5f68f0a-1adf-4de6-aa75-8d2737a25e3b" />

### CODE
```
#include <bits/stdc++.h>
using namespace std;


int main() {
    string s;
    cin >> s;

    for (int i = 0; i < s.length(); i++) {
    char c = tolower(s[i]);

    if (c != 'a' && c != 'o' && c != 'y' &&
        c != 'e' && c != 'u' && c != 'i') {
        cout << "." << c;
        }
    }

}
```
