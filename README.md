# 
 #include <bits/stdc++.h>
using namespace std;
int main() {
    int n,m;
    cin >> m>> n;
    int a[1000][1000] ={0};
int val =1;
  for(int row =0;row<=m-1;row++){
for(int col=0;col<=n-1;col++){
    a[row][col]=val;
    val=val+1;
    cout<<a[row][col]<<" ";
}
cout<<endl;
        }
    for(int col=0;col<n;col++){
    if(col%2==0){
        //even top down
        for(int row =0;row<m;row++){
            cout<< a[row][col];
        }
    }
else
{
    for(int row=m-1;row>=0;row--){
          cout<< a[row][col];
    }
}
    }
    return 0;

}
