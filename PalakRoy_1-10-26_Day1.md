### DESCRIPTION
We first find the sum to n nos. using the formula n*(n-1)/2 and then subract 2(1+2+...2^k).

### SCREENSHOT
<img width="875" height="21" alt="image" src="https://github.com/user-attachments/assets/fb4b038f-3232-4de6-bc31-c2150b77d5fe" />

### CODE
`#include <bits/stdc++.h>
using namespace std;

int main() {
    int t;
    cin >> t;
    while (t--)
    {
        long long n;
        cin >>n;
        long long sum = n * (n+1)/2;

        long long p = 1;
        while (p*2 <= n)
        {
            p*=2;
        }
        long long powersum = 2*p - 1;
        cout << sum - 2*powersum << endl;

        
        
    }
      
}
`

