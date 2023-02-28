#include<iostream>
using namespace std;

const int MAX = 10005;

int  Matrix[MAX][MAX];   
bool Visit[MAX];          
int  cnt;                                       
int  N, M;                  
void Try(int u)
{
	Visit[u] = 1;
	cnt++;

	for (int i = 1; i <= Matrix[u][0]; i++)
	{
		int v = Matrix[u][i];
		if(!Visit[v]) Try(v);
	}
}

int main()
{
	ios::sync_with_stdio(false);
    int t;
    cin >>t;
    while(t--){
        cin >> M;
        if(M == 0) cout << "NO" << endl;
        else{
            cnt = 0;

            for(int i = 0; i <= M; i++) {
                Visit[i] = false;
                for(int j = 0; j <= M; j++)
                    Matrix[i][j] = 0;
            }
            for(int i = 0; i < M - 1; i++){
                int a, b, m;
                cin >> a >> b;
                m = ++Matrix[a][0];
                Matrix[a][m] = b;
                m = ++Matrix[b][0];
                Matrix[b][m] = a;
            }
                Try(1);
                if(cnt == M) cout << "YES" << endl;
                else cout << "NO" << endl;
        }
	}

	return 0;
}
