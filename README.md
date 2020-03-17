### sorting (:
stl sort -> https://www.geeksforgeeks.org/sort-c-stl/
### stable sort
    bool fun(string i1, string i2)
    {

        if(i1.length() != i2.length())
            return  i1.length()<i2.length();
        else
        return i1<i2;



    }
    main(){
    string s;
        vector<string> unsorted;
        for(int i=0; i<5; i++)
        {
            cin>>s;
            unsorted.push_back(s);
        }
        stable_sort( unsorted.begin(), unsorted.end(),fun);
        for(int i=0; i<5; i++)
        cout<<unsorted[i]<<endl;
    }//sort string number 

