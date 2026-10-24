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
# CIEL AND DANCING
### DESCRIPTION
We first pair every guy with girl 1, so all of them dance for the first time and then we pair each girl (except girl 1) with boy 1 so all girls dance for the first time.

### SCREENSHOT
<img width="878" height="18" alt="image" src="https://github.com/user-attachments/assets/2de2fbdf-6fae-46f5-8851-717b42d2c986" />

### CODE
```
#include <bits/stdc++.h>
using namespace std;


int main() {
    int n, m;
    cin >> n >> m;

    cout << n + m -1 << endl;

    for (int i = 1; i <= n; i++){
        cout << i << " " << 1 << endl;
    }
    for (int j = 2; j <= m; j++){
        cout << 1 << " " << j << endl;
    }

}
```

