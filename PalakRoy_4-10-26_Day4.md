# RECONNAISSANCE
### DESCRIPTION
Can be solved using nested loops

### SCREENSHOT
<img width="661" height="35" alt="image" src="https://github.com/user-attachments/assets/6f18f5cc-c722-4c8b-aabe-7a24474ce60c" />

### CODE
```
#include <bits/stdc++.h>
using namespace std;

int main() {
    int n;
    long long d;
    cin >> n >> d;
    vector <long long> height(n);
    for (int i = 0; i < n; i++){
        cin >> height[i];
    }
    sort(height.begin(), height.end());

    int total = 0;
    for (int i = 0; i < n; i++){
        for (int j = i+1; j < n; j++){
            if (height[j] - height[i] <= d){
                total += 2;
            }
        }
    }
    cout << total;
    
}
```

# HOLIDAYS
### DESCRIPTION
Only need to figure out the math equation required 

### SCREENSHOT
<img width="657" height="32" alt="image" src="https://github.com/user-attachments/assets/aad4cf60-5273-40a1-9d5b-cc0cf4df1ea7" />

### CODE
```
#include <bits/stdc++.h>
using namespace std;

int main() {
    long n;
    cin >> n;

    long mino = (n/7) * 2 + max(0L, n%7-5);
    long maxo = (n/7) * 2 + min(2L, n%7);
    

    cout << mino << " " << maxo;
    
}
```
