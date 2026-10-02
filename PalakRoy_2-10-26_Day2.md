# FLAG
### DESCRIPTION
Simple problem requiring checking using nested loops (since n, m <= 100) whether there are any repitions

### SCREENSHOT
<img width="881" height="19" alt="image" src="https://github.com/user-attachments/assets/e4809246-47bd-4ee2-9c10-3e095165566e" />

### CODE
```
#include <bits/stdc++.h>
using namespace std;

int main() {
    int n, m;
    cin >> n >> m;

    vector<string> flag(n);
    for (auto &row : flag)
        cin >> row;

    for (int i = 0; i < n; ++i) {
        for (int j = 1; j < m; ++j) {
            if (flag[i][j] != flag[i][0]) {
                cout << "NO";
                return 0;
            }
        }

        if (i > 0 && flag[i][0] == flag[i - 1][0]) {
            cout << "NO";
            return 0;
        }
    }

    cout << "YES";
    return 0;
}
```

# WET SHARK AND ODD AND EVEN
### DESCRIPTION
We add the nos and find the max sum, which if even is printed but if odd, we subtract the smallest odd no given making the sum 
even. 

### SCREENSHOT
<img width="662" height="38" alt="image" src="https://github.com/user-attachments/assets/469fd316-4fed-48c9-b473-0a1499515fa7" />

### CODE
```
#include <bits/stdc++.h>
using namespace std;


int main() {
    int n;
    cin >> n;

    long long sum = 0;
    long long minodd = LLONG_MAX;

    for (int i = 0; i < n; i++){
        long long a;
        cin >> a;

        sum += a;

        if (a % 2 != 0){
            minodd = min(minodd, a);
        }
    }
    if (sum % 2 == 0){
        cout << sum;
    }else{
        cout << sum - minodd;
    }
        
}

```

# AVERAGE NUMBERS
### DESCRIPTION
An element will satisfy the condition when the total sum of all elements(S) is divisible by n, basically a[i] = S/n

### SCREENSHOT
<img width="883" height="17" alt="image" src="https://github.com/user-attachments/assets/fb4b11fa-eae2-461e-98a0-5df8454f631f" />

### CODE
```
#include <bits/stdc++.h>
using namespace std;

int main() {
    int n;
    cin >> n;

    vector<int> a(n);
    long long sum = 0;

    for (int &x : a) {
        cin >> x;
        sum += x;
    }

    vector<int> ans;

    if (sum % n == 0) {
        long long mean = sum / n;

        for (int i = 0; i < n; ++i) {
            if (a[i] == mean)
                ans.push_back(i + 1);
        }
    }

    cout << ans.size() << '\n';

    for (int i : ans)
        cout << i << ' ';
    cout << endl;

    return 0;
}
```
