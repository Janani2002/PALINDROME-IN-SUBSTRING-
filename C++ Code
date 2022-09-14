// PALINDROME IN SUBSTRING 

#include <iostream>
using namespace std;
int main()
{
    string s;
cin>>s;
        int n = s.length();
        if(n==1) 
        cout<<s;
        string ans = "";
        int low, high;
        int start_index;
        int max_length = 0;
        for(int i = 1; i < n; i++)
        {
            low = i - 1;
            high = i + 1;
            while(low >= 0 && high < n && s[low] == s[high])
            {
                if(max_length < high - low + 1)
                {
                    max_length = high - low + 1;
                    start_index = low;
                }
                --low;
                ++high;
            }
            low = i - 1;
            high = i;
         }
        if(max_length == 0)
        {
        ans += s[0];
            cout<< ans;
        }
        for(int i = start_index; i < start_index + max_length; i++)
        {
            ans += s[i];
        }
        cout<< ans;
return 0;
    }
