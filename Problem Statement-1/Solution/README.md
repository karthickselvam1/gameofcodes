#include<iostream>
using namespace std;

int main(){
    int t;
    cin>>t;
    while(t--)
    {
        int n,a,b,k;
        cin>>n>>a>>b>>k;
        for(int i=1;i<=n;i++)
        {
            if(i%a==0 and i%b==0)
            continue;
            else if(i%a==0)
            k--;
            else if(i%b==0)
            k--;
        }
        if(k<=0)
        cout<<"Win\n";
        else
        cout<<"Lose\n";
    }
}

