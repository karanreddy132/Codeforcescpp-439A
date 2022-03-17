# Codeforcescpp-439A
#include <bits/stdc++.h>

using namespace std;

int main(){
  int n,d,ele,sum(0);
  cin >> n >> d;
  for(int i=0;i<n;i++){
    cin >> ele;
    sum+=ele;
  }
  
  int time = sum+10*(n-1);
  if(time > d){
    cout << -1;
  }
  else{
    cout << 2*(n-1) + (d-time)/5;
  }
  return 0;
}
