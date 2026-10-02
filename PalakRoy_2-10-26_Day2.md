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
