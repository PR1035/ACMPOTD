# PASSWORD CHECK
### DESCRIPTION
You just go through a list and ensure all of the conditions are present

### SCREENSHOT
<img width="879" height="24" alt="image" src="https://github.com/user-attachments/assets/4f278a02-7ecd-45cb-b692-ff25fe509131" />

### CODE
```
#include <bits/stdc++.h>
using namespace std;


int main() {
    string s;
    cin >> s;

    if (s.size() < 5){
        cout << "Too weak";
        return 0;
    }
    bool upper = false, lower = false, digit = false;
    for (int i = 0; i < s.size(); i++){
        if (isupper(s[i])) upper = true;
        else if (islower(s[i])) lower = true;
        else if (isdigit(s[i])) digit = true;
    }
    if (upper && lower && digit){
        cout << "Correct";
    }else{
        cout << "Too weak";
    }

}
```

