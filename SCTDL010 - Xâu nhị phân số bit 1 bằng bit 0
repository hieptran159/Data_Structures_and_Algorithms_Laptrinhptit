// Bai nay phai de cac bit bat dau tu 1 truoc moi dung :))
#include <bits/stdc++.h>
using namespace std;

void AddBitToString(int n, string s, int bit1, int bit0)
{
    // Dieu kien dung la khi so bit them vao = n
    if (s.length() == n)
    {
        cout << (s) << " ";
        return;
    }

    // Neu so bit 1 < n/2 thi ta them bit 1 vao chuoi, dong thoi tang bien dem bit1 len 1 don vi
    if (bit1 < n / 2)
        AddBitToString(n, s + "1", bit1 + 1, bit0);

    // Neu so bit 0 < n/2 thi ta them bit 1 vao chuoi, dong thoi tang bien dem bit0 len 1 don vi
    if (bit0 < n / 2)
        AddBitToString(n, s + "0", bit1, bit0 + 1);
}

int main()
{
    int test;
    cin >> test;
    while (test--)
    {
        string s = "";
        int n;
        cin >> n;
        if (n < 1 || n & 1)
        {
            cout << -1 << endl;
        }
        else
        {
            AddBitToString(n, s, 0, 0);
            cout << endl;
        }
    }
    return 0;
}
