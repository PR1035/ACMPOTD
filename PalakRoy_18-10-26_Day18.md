# Stones on the Table
### DESCRIPTION
In this, I used a stack and added the first color to top of the stack. Then we move on to the next letter of the string and check if matches the top of the stack. If it does, we do ct+=1 and pop the top. 

### SCREENSHOT
<img width="872" height="21" alt="image" src="https://github.com/user-attachments/assets/b7af0ef1-02e4-4826-99f1-86825dda26ce" />

### CODE
```
#include <bits/stdc++.h>
using namespace std;

int main() {
    int n;
    cin >> n;
    string s;
    cin >> s;
    stack <char> st;
    st.push(s[0]);
    int ct = 0;
    for (int i = 1; i < n; i++){
        if (st.top() == s[i]){
            ct++;
            st.pop();
        }
        st.push(s[i]);
    }
    cout << ct;
}
```

# Palindromic Times
