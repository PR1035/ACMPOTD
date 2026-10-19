<img width="883" height="22" alt="image" src="https://github.com/user-attachments/assets/71e133bd-1f43-4054-9174-752453798f17" /># BEAUTIFUL YEAR
### DESCRIPTION
We loop till from the year + 1(+1 incase it itself is a year with distinct digits) till 9999 and find the distinct year and print that. To find if digits are distinct in a no. we have a function where we convert the int to a string and put all characters of the string in a unordered set of chars. Then we return whether they have the same sizes.

### SCREENSHOT
<img width="875" height="27" alt="image" src="https://github.com/user-attachments/assets/951a6f53-d556-4095-9d43-665858125011" />

### CODE
```
#include <bits/stdc++.h>
using namespace std;

bool different(int y){
    string s = to_string(y);
    unordered_set <char> digits(s.begin(), s.end());
    bool value = (s.size() == digits.size());
    return value;
}

int main() {
    int y;
    cin >> y;

    for (int i = y+1; i < 9999; i++){
        if (different(i)){
            cout << i;
            return 0;
        }
    }
}
```

# LUCKY SUM OF DIGITS
### DESCRIPTION
Since there is no limit to the no of digits, we move the loop in backwards. we only check digits with 4 and 7. 

### SCREENSHOT
<img width="883" height="22" alt="image" src="https://github.com/user-attachments/assets/4ff6b43e-d280-4437-8e07-ab52ef9a87ea" />

### CODE
```
#include <bits/stdc++.h>
using namespace std;


int main() {
    int n;
    cin >> n;
    
    for (int seven = n/7; seven >= 0; seven--){
        int rem = n - (7*seven);
         if (rem % 4 ==0){
            int four = rem / 4;
            cout << string(four, '4') << string(seven, '7');
            return 0;
         }
    }
    cout << -1;
}
```
