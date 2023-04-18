#include <iostream>
#include <string>
using namespace std;

int depth(string s, int& index) {
    if (s[index] == 'l') {
        return 0;
    } else if (s[index] == 'n') {
        index++;
        int left_depth = depth(s, index);
        index++;
        int right_depth = depth(s, index);
        return max(left_depth, right_depth) + 1;
    } else {
        return -1;
    }
}

int main() {
    int t;
    cin >> t;
    while (t--) {
        int n;
        cin >> n;
        string s;
        cin >> s;
        int index = 0;
        int d = depth(s, index);
        
            cout << d << endl;
        
    }
    return 0;
}
