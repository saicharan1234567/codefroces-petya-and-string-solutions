# codefroces-solutions

#include <bits/stdc++.h>
#include<ctype.h>
using namespace std;

int main() {
	string s1,s2;
	cin>>s1;
	cin>>s2;
	int cnt=0;
	for(int i=0;i<s1.length();i++){
		s1[i]=tolower(s1[i]);
		s2[i]=tolower(s2[i]);
		if(s1[i]>s2[i]){
			cout<<"1"<<endl;
			break;
		}
		else if(s1[i]<s2[i]){
			cout<<"-1"<<endl;
			break;
		}
		else
		    cnt++;
	}
	if(s1.length()==cnt)
	     cout<<"0"<<endl;
	
	return 0;
}
