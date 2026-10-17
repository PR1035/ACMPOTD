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

# YOUNG PHYSICIST
### DESCRIPTION
To check if equilibrium is present we add the x forces with each other and do the same with y and z

### SCREENSHOT
<img width="889" height="20" alt="image" src="https://github.com/user-attachments/assets/4b2a7c02-a8d1-4b36-a3cf-805efaf9341a" />

### CODE
```
#include <bits/stdc++.h>
using namespace std;

int main() {
    int n;
    cin >> n;

    vector <int> x(n), y(n), z(n);
    for (int i = 0; i < n; i++){
        cin >> x[i] >> y[i] >> z[i];
    }
    int sumx = 0, sumy = 0, sumz = 0;
    for (int i = 0; i < n; i++){
        sumx += x[i];
        sumy += y[i];
        sumz += z[i];
    }
    if (sumx == 0 && sumy == 0 && sumz == 0){
        cout << "YES";
    }else{
        cout << "NO";
    }
}
```
