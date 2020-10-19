#include<iostream>
using namespace std;

int main()
{
    int r = 4,c=5;
    int cap[4];
    int req[5];
    int a[3][4];
    int t1=0,t2=0;
    cout<<"Enter the capacity"<<endl;
    for(int i=0;i<3;i++)
    {

       cin>>cap[i];
       t1 = t1 + cap[i];
    }
    cout<<"Enter the req."<<endl;
    for(int i=0;i<4;i++)
    {
        cin>>req[i];
        t2 = t2 + req[i];
    }
    //----------------------------------------------------------------------------------------
    if(t1==t2)
    {
        cout<<"Transportation  problem is balanced"<<endl;
        cout<<"-------------------------------------------------"<<endl;
        cout<<"Enter the data"<<endl;
        for(int i=0;i<3;i++)
        {
            for(int j=0;j<4;j++)
            {
                cin>>a[i][j];
            }
        }
        //---------------------------------------------------------------------
        int sum = 0;
        int m=0,n=0;
        for(int i=0;i<6;i++)
        {

        if(cap[m]>req[n])
        {
            cap[m] = cap[m]-req[n];
            int value = req[n]*a[m][n];
            req[n] = 0;
            sum = sum+value;

            n++;
        }
         else
        {
            req[n] = req[n]-cap[m];
            int value = cap[m]*a[m][n];
            cap[m] = 0;
            sum = sum+value;

            m++;
        }
        }
        cout<<"----------------------------------------------------------"<<endl;
        cout<<"Minimum transportation cost"<<sum;
    }
    else{
        cout<<"Transportation problem is unbalanced"<<endl;
    }
    //------------------------------------------------------------------------
}
