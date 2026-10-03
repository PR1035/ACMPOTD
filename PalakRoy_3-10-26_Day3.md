# SECOND ORDER STATISTICS
### DESCRIPTION
Simple problem which required usage of set(so that elements are sorted and there are no duplicates) and then finding the 2nd element of the set.

### SCREENSHOT
<img width="875" height="18" alt="image" src="https://github.com/user-attachments/assets/4fe4e28d-161f-49ae-93c4-f2bd123b00b2" />

### CODE
```
#include <bits/stdc++.h>
using namespace std;


int main() {
    int n;
    cin >> n;

    set<int> a;
    for (int i = 0; i < n; i++){
        int s;
        cin >> s;
        a.insert(s);
    }

    if (a.size() >= 2){
        cout << *next(a.begin(), 1);
    }else{
        cout << "NO";
    }
    
}
```

# THE TIME
### DESCRIPTION
The only complicated portion was figuring out how to output the single digit numbers, which turned out can be done by using inbuilt functions like setw and setfill

### SCREENSHOT
<img width="875" height="18" alt="image" src="https://github.com/user-attachments/assets/1239b520-1523-4a7c-be51-3ff688e18cc6" />

### CODE
```
#include <bits/stdc++.h>
using namespace std;


int main() {
    string s;
    cin >> s;

    string s1 = s.substr(0, 2);
    string s2 = s.substr(3, 2);

    int n;
    cin >> n;

    int h = stoi(s1);
    int m = stoi(s2);

    m += n;
    h += m/60;
    m %= 60;
    h %= 24;

    cout << setfill('0') << setw(2)  << h << ":" << setw(2) <<  m;
    
}
```
