#include <bits/stdc++.h>
using namespace std;
string bin;

void numnext () {
	int l=bin.length(), check=1, k;
	for (int i=l-1; i>=0; i--) 
		if (bin[i]=='0') {
			check=0;
			k=i;
			break;
		}
	bin[k]='1';
	for (int i=k+1; i<=l; i++)
		bin[i]='0';	
	if (check) {
		for (int i=0; i<l; i++)
			cout <<0;
	} 	else {
			cout <<bin;
		}
	cout <<endl;
	
}

int main () {
	int t;
	cin >>t;
	while (t--) {
		cin >>bin;
		numnext ();
	}
	return 0;
}
