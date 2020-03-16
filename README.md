###  Sive of Eratosthenes
    #include<bits/stdc++.h>
    using namespace std;
    int fun(int n)
    {

        int primes[n+1];
        primes[0]=0;
        primes[1]=0;
        for(int i=2; i<=sqrt(n); i++)
        {
             primes[i]=1;
            for(int j=i; j*i<=n; j++)
             primes[j]=0;
        }
        return primes[n];
    }
    
    int main()
    {
        int n,x;
        cin>>n;
        x=fun(n);
        if(x == 0)
        cout<<"not prime"<<endl;
        else
        cout<<"prime"<<endl;

    }
time complexity : o(n log log n)
tutorial:https://www.youtube.com/watch?v=eKp56OLhoQs
