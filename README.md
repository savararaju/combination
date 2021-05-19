# combination


#include<iostream>
#include<bits/stdc++.h>
using namespace std;
int n=4;
int a[4]={2,3,6,7};
int N=7;

void printarraycomb(int ind, int N, vector<int>&ds)
{
    if(ind==n)
    {
        if(N==0)
        {
            for(auto itr:ds)
            {
                cout<<itr<<" ";
            }
         cout<<"\n ";
        }
        return;
    }
    if(a[ind]<=N)
    {
        ds.push_back(a[ind]);
    printarraycomb(ind,N-a[ind],ds);
    ds.pop_back();
    }
   printarraycomb(ind+1,N,ds);
}

int main()
{
    vector<int>aditya;
      printarraycomb(0,N,aditya)   ;
    return 0;
}
    
    
    
    
    
    
    ------------------------------------------------------
    
    #include<iostream>
#include<bits/stdc++.h>
using namespace std;
int n=7;
int a[7]={10,1,2,7,6,1,5};
int N=8;

void printarraycomb(int ind, int N, vector<int>&ds)
{
    if(ind==n)
    {
        if(N==0)
        {
            for(auto itr:ds)
            {
                cout<<itr<<" ";
            }
         cout<<"\n ";
        }
        return;
    }
    if(a[ind]<=N)
    {
        ds.push_back(a[ind]);
    printarraycomb(ind,N-a[ind],ds);
    ds.pop_back();
    }
   printarraycomb(ind+1,N,ds);
}

int main()
{
    vector<int>aditya;
      printarraycomb(0,N,aditya)   ;
    return 0;
}
